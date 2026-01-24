---
title: "Machine-Readable Conventions"
type: "guide"
layer: "00_scope"
sequence: 45
purpose: "Document parsing rules and conventions for AI systems processing GFN content"
audience: "AI systems, automated indexing tools, and documentation generators"
epistemic_status: Consensus
tags: [reference, machine-readable, conventions, parsing]
dependencies: ["10_epistemic_status.md", "20_taxonomy.md", "30_entry_template.md", "40_what_would_change_our_minds.md", "50_adversarial_scenarios.md"]
related_documents:
  - based_on: ["25_taxonomy_index.md", "35_relationships_map.md"]
  - used_with: ["entry_validation_checklist.md", "_examples/"]
last_updated: "2026-01-24"
version: "1.0"
---

# Machine-Readable Conventions for 00_scope

This document specifies how AI systems, automated tools, and documentation generators should parse and interpret content in the GFN `00_scope` layer.

---

## YAML Frontmatter Specification

All files in `00_scope` include a YAML frontmatter block at the top, delimited by `---`.

### Required Fields

```yaml
---
title: string                     # Human-readable file title
type: enum                       # [framework|template|reference|guide]
layer: string                    # Always "00_scope" for this layer
sequence: number                 # 10, 20, 25, 30, 35, 40, 45, 50
purpose: string                  # Single sentence describing purpose
audience: string                 # Target readers
epistemic_status: enum           # [Speculative|Theoretical|Empirical|Consensus]
confidence: number (0-100)       # Confidence percentage
tags: array<string>              # Functional tags
dependencies: array<string>      # Files this depends on (paths or filenames)
last_updated: string (ISO 8601)  # YYYY-MM-DD format
version: string (semver)         # e.g., "1.0", "1.1", "2.0"
---
```

### Optional Fields

```yaml
related_documents:               # Cross-references (object with keys)
  - prerequisite: string         # Files to read first
  - next: string                 # Recommended next file
  - used_by: array<string>       # Files that use this
  - see_also: array<string>      # Related files
  - examples: string or array    # Pointer to examples
  - protects: array<string>      # Files this defends
  - validates: array<string>     # Claims/rules this validates
```

### Example Frontmatter

```yaml
---
title: "Taxonomy and Classification Framework"
type: "framework"
layer: "00_scope"
sequence: 20
purpose: "Define categorization logic for all GFN entries"
audience: "Contributors, curators, and AI systems"
epistemic_status: Consensus
confidence: 95
tags: [framework, operational, classification, taxonomy]
dependencies: ["10_epistemic_status.md"]
related_documents:
  - prerequisite: "10_epistemic_status.md"
  - used_by: "30_entry_template.md"
  - see_also: ["40_what_would_change_our_minds.md"]
last_updated: "2026-01-24"
version: "1.0"
---
```

### Parsing Rules

- **Parse YAML**: Use standard YAML parser (YAML 1.2)
- **Validate types**: Ensure fields match specified types
- **Check dependencies**: Verify all listed dependencies exist
- **Extract tags**: Tags stored as plain strings in YAML; display with `#` prefix when needed
- **Date format**: Always ISO 8601 (YYYY-MM-DD)
- **Sequence numbers**: Must be in range [10, 20, 25, 30, 35, 40, 45, 50]
- **Important**: Tags in YAML arrays MUST NOT include `#` symbol (causes parser error)

---

## Document Structure Parsing

After YAML frontmatter, documents follow this structure:

### Expected Header Hierarchy

```
# [Document Title]           (H1) - Usually same as YAML title

## Document Summary         (H2) - Brief overview
  (paragraph content)

## Related Documents        (H2) - Cross-references
  (markdown list)

---  (horizontal rule separating metadata from content)

# [Main Section Title]      (H1) - Start of substantive content

## Subsection              (H2)

### Subsubsection          (H3)

...
```

### Parsing Rules

- **H1**: Appears once at top of document (after metadata section)
- **H2**: Used for major sections (Related Documents, then content sections)
- **H3**: Used for subsections within major sections
- **H4+**: Rarely used; indicates deep nesting (usually in complex tables or examples)

### Document Sections to Extract

All files contain:
1. **YAML Frontmatter** (lines 1-18 approx)
2. **Document Summary** (H2 section)
3. **Related Documents** (H2 section)
4. **Horizontal Rule** (`---`)
5. **Main Content** (H1 followed by H2/H3 sections)

---

## Tag System Specification

### Tag Format in YAML Frontmatter

**IMPORTANT**: In YAML frontmatter arrays, do NOT include the `#` symbol. Tags are stored as plain lowercase strings with hyphens.

**✅ CORRECT FORMAT**:
```yaml
tags: [alignment, foundational, epistemic, meta]
tags: [framework, operational, classification, taxonomy]
```

**❌ INCORRECT FORMAT** (causes YAML parser error):
```yaml
tags: [#alignment, #foundational, #epistemic, #meta]
tags: [#framework, #operational, #classification, #taxonomy]
```

**Rationale**: YAML uses `#` for comments. To avoid parser errors, omit `#` in array values. The `#` prefix is added when displaying tags to users/documentation.

### Standard Tags

All tags use format: `#lowercase-with-hyphens` (display format; stored without `#` in YAML)

#### Framework Tags
- `#framework` - Meta-frameworks, foundation documents
- `#foundational` - Core principles
- `#meta` - Meta-level, self-referential
- `#operational` - Practical, operational rules

#### Domain Tags
- `#alignment` - AI value alignment
- `#governance` - Governance and institutions
- `#coordination` - Coordination problems
- `#verification` - Verification and monitoring
- `#technical` - Technical solutions
- `#institutional` - Institutional solutions
- `#epistemic` - Epistemology, knowledge
- `#classification` - Classification systems
- `#taxonomy` - Taxonomy/categories

#### Quality/Status Tags
- `#reference` - Reference material
- `#quick-lookup` - Designed for fast reference
- `#index` - Index or mapping document
- `#guide` - How-to or instructional
- `#exemplar` - Example or exemplary
- `#adversarial` - Adversarial scenarios
- `#resilience` - Resilience mechanisms
- `#security` - Security considerations

#### Parsing Rules

- Extract all tags (words starting with `#` in metadata sections)
- Normalize to lowercase-with-hyphens
- Store as array of strings
- Cross-reference against approved tag list

---

## Cross-Reference and Link Parsing

### Expected Link Formats

All cross-references use Markdown link syntax:

```markdown
[Display Text](target-file.md)
[Display Text](path/to/target-file.md)
[Display Text](../other-layer/target-file.md)
```

### Link Resolution Rules

1. **Relative links**: Resolve relative to current file directory
2. **Same-layer links**: Typically reference other `00_scope/` files
3. **Cross-layer links**: Reference `10_hypotheses/`, `20_mechanisms/`, etc.
4. **Validation**: Check that target file exists

### Common Link Patterns

In `30_entry_template.md`:
```markdown
See `20_taxonomy.md` for classification tags.
Reference `40_what_would_change_our_minds.md` for falsifiability requirements.
Examples in `_examples/hypothesis_A1_good.md`
```

---

## Markdown Table Parsing

Tables in quick-reference documents (e.g., `25_taxonomy_index.md`) are designed for machine parsing:

### Table Specifications

- **Format**: Standard Markdown table (pipes and hyphens)
- **Headers**: First row contains column names
- **Data rows**: Subsequent rows contain data
- **Pipes**: Use `|` to delimit cells
- **Content**: Can contain inline code, bold, links

### Example Table

```markdown
| Category | Type | Definition | Example |
|----------|------|-----------|---------|
| A1 | Internal | Value Alignment | Mismatch in objectives |
```

### Parsing Rules

- Parse using standard Markdown table parser
- Trim whitespace from cells
- Interpret inline formatting (bold, code, links)
- Handle cells with special characters using escape sequences

---

## Entry Template Validation Rules (For Machines)

When parsing entries created with `30_entry_template.md`, validate the following:

### Required Sections (All Must Present)

1. **Metadata** (H3 or bold text)
   - Must include: Title, Category, Epistemic Status, Confidence
   
2. **Claim / Hypothesis** (H3)
   - Must be < 1000 words
   - Should be a clear, testable statement
   
3. **Mechanism** (H3)
   - Must explain causal chain
   - Should be 300-600 words
   
4. **Observable Predictions** (H3)
   - Must list 2+ predictions
   - Each prediction should have observable metric
   
5. **Counterarguments** (H3)
   - Must present objections
   - Should not be strawmanned (AI can detect strawmanning)
   
6. **Failure Modes** (H3)
   - Must identify when mechanism fails
   - Should be realistic scenarios
   
7. **What Would Change My Mind** (H3)
   - **MANDATORY**: Must be present
   - Should list 3+ conditions for revision
   
8. **References** (H3)
   - Must have 5+ citations
   - Should include diverse sources

### Optional but Recommended Sections

- Uncertainty / Credence
- Response Patterns
- Examples
- Related Entries

### Validation Algorithm

```
FOR EACH entry:
  1. Extract YAML frontmatter
  2. Verify required fields present (title, category, status)
  3. Verify tags are from approved list
  4. Count section headers (H3)
  5. Check minimum sections present: 6 mandatory + "What Would Change My Mind"
  6. Count references: must be >= 5
  7. Check for circular logic patterns
  8. Verify no unfalsifiable claims
  9. Flag any missing "What Would Change My Mind" section (RED FLAG)
  10. Return validation report
```

---

## Entry Metadata Parsing

In entry files, metadata appears at top in formats like:

```markdown
**Title**: Value Alignment Failure
**Category**: A1
**Epistemic Status**: [Theoretical]
**Confidence**: 65%
**Tags**: #alignment #existential-risk #long-term
```

### Parsing Rules

- Extract lines starting with `**[Field Name]**:`
- Parse following value according to field type
- Convert percentage strings to numbers (e.g., "65%" → 65)
- Parse epistemic status from brackets: `[Theoretical]`
- Parse tags as comma-separated or space-separated list

---

## Special Patterns

### Falsifiability Pattern

Look for section titled "What would change my mind" or similar:
- Should contain conditional statements
- Should propose testable criteria
- Should not be vague or unfalsifiable

### Confidence Calibration Pattern

Confidence claims should appear in forms like:
- "65% confidence"
- "[Low / Moderate / High] confidence"
- Numerical ranges (e.g., "40-70%")

### Reference Format Variety

References may appear as:
- Markdown links: `[Author, Year](url)`
- Plain text citations: "Bostrom (2014), Superintelligence"
- In-text citations with footnotes
- Bibliography section

Parsers should be flexible in extracting bibliographic data.

---

## Error Handling

### Validation Warnings (Yellow Flags)

- Missing optional fields
- Unusually short sections (< 50 words)
- Unusually long sections (> 2000 words)
- References to non-existent files
- Broken Markdown links
- Malformed YAML frontmatter (recoverable)

### Validation Errors (Red Flags)

- Missing mandatory sections
- < 5 references
- "What would change my mind" section missing
- Unfalsifiable claims (detected via keyword analysis)
- Circular dependencies in stated assumptions
- Malformed YAML frontmatter (non-recoverable)

### Reporting

- Generate validation reports with line numbers
- Suggest fixes for common issues
- Preserve original content for human review

---

## For Documentation Generators

### Extracting Data

1. Parse YAML frontmatter for metadata
2. Extract H2 sections and treat as major categories
3. Extract all tables for structured data
4. Extract links for cross-reference mapping
5. Extract tags for categorization

### Building Indices

- Create tag index: tag → [files]
- Create category index: category → [entries]
- Create dependency graph: file → dependencies
- Create reverse dependency graph: file → dependents

### Generating Documentation

- Use YAML `purpose` and `audience` for descriptions
- Use `related_documents` for cross-references
- Use headers for table of contents
- Use tags for filtering and search

---

## AI System Guidance

### What You Should Do

✅ Parse YAML frontmatter for metadata  
✅ Extract classification tags and use for organization  
✅ Validate entries against required sections  
✅ Build indexes and cross-reference maps  
✅ Preserve context when reusing material  
✅ Report validation errors to maintainers  

### What You Should NOT Do

❌ Modify files without explicit permission  
❌ Ignore missing "What would change my mind" sections  
❌ Treat all epistemic statuses as equally reliable  
❌ Create new tags not in approved list  
❌ Extract and republish without attribution  

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2026-01-24 | Initial specification |

---

Last Updated: 2026-01-24