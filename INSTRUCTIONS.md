# Raw Source Collection Instructions

**Project:** Content Audit - Official Source Raw Material Collection  
**For:** Sourabh  
**Date:** 2025-11-13

---

## Overview

This guide provides step-by-step instructions for collecting raw source material from official government websites. The goal is to gather **accurate, complete, and properly formatted** raw statutory and regulatory text for all 18 approved sources.

---

## Table of Contents

1. [What Are Raw Sources?](#what-are-raw-sources)
2. [Collection Methods](#collection-methods)
3. [File Naming Conventions](#file-naming-conventions)
4. [Metadata Header Requirements](#metadata-header-requirements)
5. [Step-by-Step Collection Process](#step-by-step-collection-process)
6. [Quality Verification Checklist](#quality-verification-checklist)
7. [Organizing Existing Files](#organizing-existing-files)
8. [Common Issues & Solutions](#common-issues--solutions)

---

## What Are Raw Sources?

**Raw sources** are the **unprocessed, original text** directly from official government websites. They serve as the authoritative foundation for content verification.

**Characteristics of Raw Sources:**
- ✅ Complete statutory/regulatory text from official URLs
- ✅ No summarization or interpretation
- ✅ No processing or formatting (except markdown conversion)
- ✅ Includes all sections, subsections, and amendments
- ✅ Metadata documenting source URL and collection date

**Why We Need Them:**
- Verify accuracy of processed course content
- Audit for completeness
- Reference for updates and changes
- Foundation for 50-state expansion

---

## Collection Methods

### Method 1: Federal Statutes (USC - United States Code)

**Official Sources:**
- **Primary:** https://www.govinfo.gov (Government Publishing Office)
- **Alternative:** https://uscode.house.gov (U.S. House of Representatives)

**Process:**
1. Navigate to the specific title and chapter
2. Select "Text" or "HTML" format (easier to copy)
3. Copy entire chapter text (all sections)
4. Paste into text editor
5. Save as markdown (.md) file

**Example:** Fair Housing Act (42 USC §3601)
- URL: https://www.govinfo.gov/content/pkg/USCODE-2021-title42/html/USCODE-2021-title42-chap45.htm
- Copy all sections from §3601 through the end of Chapter 45

---

### Method 2: Federal Regulations (CFR - Code of Federal Regulations)

**Official Source:**
- **Primary:** https://www.ecfr.gov (Electronic Code of Federal Regulations)

**Process:**
1. Navigate to specific title and part
2. Use "Download" or "Print" feature for complete text
3. Copy text from browser
4. Clean up formatting (remove navigation elements)
5. Save as markdown (.md) file

**Example:** Regulation X (12 CFR §1024)
- URL: https://www.ecfr.gov/current/title-12/chapter-X/part-1024
- Copy all subparts (A, B, C, etc.)

**Note:** CFR regulations may have official PDFs available for download - save these to `binary_files/` folder.

---

### Method 3: Virginia Statutes

**Official Source:**
- **Primary:** https://law.lis.virginia.gov/vacode/ (Virginia Legislative Information System)

**Process:**
1. Navigate to specific title and chapter
2. Virginia LIS provides chapter-by-chapter view
3. Copy complete chapter text (all articles and sections)
4. Alternative: Use "Print View" for cleaner text
5. Save as markdown (.md) file

**Example:** Virginia RLTA (§55.1-1200 et seq.)
- URL: https://law.lis.virginia.gov/vacodefull/title55.1/chapter12/
- Copy all articles (1-7) with all sections

---

### Method 4: Virginia Regulations (VAC - Virginia Administrative Code)

**Official Source:**
- **Primary:** https://law.lis.virginia.gov/admincode/ (Virginia Legislative Information System)

**Process:**
1. Navigate to specific title, agency, and chapter
2. Copy all parts and sections
3. Regulations may span multiple pages - ensure completeness
4. Save as markdown (.md) file

**Example:** VA Real Estate Board Regulations (18 VAC 135-20)
- URL: https://law.lis.virginia.gov/admincode/title18/agency135/chapter20/
- Copy all parts (I-VI)

---

### Method 5: Professional Standards (NAR)

**Official Source:**
- **Primary:** https://www.nar.realtor/ (National Association of Realtors)

**Process:**
1. Navigate to governing documents section
2. Download official PDF (preferred)
3. If text version available, copy complete text
4. Save both PDF (to binary_files/) and text version

**Example:** NAR Code of Ethics 2025
- Official PDF should already exist in workspace
- Verify it's the 2025 version

---

## File Naming Conventions

### Format
```
[source_type]_[citation]_raw.md
```

### Examples

**Federal Statutes:**
- `fair_housing_act_42usc3601_raw.md`
- `respa_12usc2601_raw.md`
- `tila_15usc1601_raw.md`
- `ecoa_15usc1691_raw.md`

**Federal Regulations:**
- `regulation_x_12cfr1024_raw.md`
- `regulation_z_12cfr1026_raw.md`

**Virginia Statutes:**
- `virginia_fhl_36-96_raw.md`
- `virginia_rlta_55.1-1200_raw.md`
- `virginia_pda_55.1-700_raw.md`

**Virginia Regulations:**
- `18vac135-20_raw.md`

**Professional Standards:**
- `nar_code_of_ethics_2025_raw.md`

### Rules
- All lowercase
- Underscores between words
- Include statute/regulation citation numbers
- Always end with `_raw.md`
- No spaces or special characters

---

## Metadata Header Requirements

**Every raw source file MUST include a metadata header** at the top of the file before the actual statutory text.

### Template

```markdown
# [Source Name] - Raw Source Material

**Source URL:** [Full official URL where text was retrieved]  
**Retrieved Date:** [YYYY-MM-DD]  
**Collected By:** Sourabh  
**Source Type:** [Official Government Website / Official PDF / etc.]  
**Verification Status:** [Pending Review / Verified]

**Citation:** [Legal citation - e.g., 42 USC §3601 et seq.]

**Notes:** [Any important notes about collection - e.g., "Retrieved from govinfo.gov HTML version" or "PDF dated 2025-06-05"]

---

[Begin actual statutory/regulatory text here]
```

### Example (Fair Housing Act)

```markdown
# Fair Housing Act - Raw Source Material

**Source URL:** https://www.govinfo.gov/content/pkg/USCODE-2021-title42/html/USCODE-2021-title42-chap45.htm  
**Retrieved Date:** 2025-11-13  
**Collected By:** Sourabh  
**Source Type:** Official Government Website (govinfo.gov - HTML format)  
**Verification Status:** Pending Review

**Citation:** 42 USC §3601 et seq. (Chapter 45 - Fair Housing)

**Notes:** Retrieved from U.S. Government Publishing Office official website. HTML version of 2021 USC edition.

---

CHAPTER 45—FAIR HOUSING

Sec.
3601. Declaration of policy.
3602. Definitions.
...

[Continue with full statutory text]
```

---

## Step-by-Step Collection Process

### Step 1: Select a Source from ASSIGNMENTS.md

- Start with **HIGH PRIORITY** sources (verified sources needing raw material)
- Fair Housing Act, RESPA, NAR Code of Ethics

### Step 2: Visit Official URL

- Use the URL provided in ASSIGNMENTS.md
- Verify you're on an official .gov or authorized site
- Check for "current as of" date if available

### Step 3: Copy Complete Text

**For Statutes:**
- Copy ALL sections from beginning to end
- Include section numbers and titles
- Don't skip subsections

**For Regulations:**
- Copy ALL subparts and appendices
- Include section numbers
- Verify completeness

### Step 4: Create New File

- Open text editor (TextEdit, VS Code, etc.)
- Create new file with proper naming convention
- Save in appropriate subdirectory:
  - `federal_statutes/`
  - `federal_regulations/`
  - `professional_standards/`
  - `virginia_sources/statutes/`
  - `virginia_sources/regulations/`

### Step 5: Add Metadata Header

- Use the metadata template above
- Fill in ALL required fields:
  - Source URL (exact URL you visited)
  - Retrieved Date (today's date: YYYY-MM-DD format)
  - Collected By: Sourabh
  - Source Type
  - Citation
  - Any relevant notes

### Step 6: Paste Statutory Text

- Paste the copied text below the metadata header
- Ensure separator line (`---`) between metadata and text
- No need to clean up formatting extensively - keep it raw

### Step 7: Download PDF (If Available)

- Many sources have official PDF versions
- Download PDF to your computer
- Save to appropriate `binary_files/` subdirectory:
  - `binary_files/federal_statutes/`
  - `binary_files/federal_regulations/`
  - `binary_files/professional_standards/`
  - `binary_files/virginia_sources/`
- Use descriptive filename matching the .md file

### Step 8: Self-Verify

Use the Quality Verification Checklist (below) before marking complete.

### Step 9: Update ASSIGNMENTS.md

- Check off completed items in source's checklist
- Update progress tracking section
- Mark source as complete

---

## Quality Verification Checklist

Before marking a source complete, verify:

### Completeness
- [ ] All sections/articles included (check official source for section list)
- [ ] No sections skipped
- [ ] All subsections and paragraphs included
- [ ] Appendices included (if applicable for regulations)

### Accuracy
- [ ] Text matches official source exactly
- [ ] No copy/paste errors or truncation
- [ ] Section numbers correct
- [ ] All special characters rendered correctly

### Metadata
- [ ] Source URL is complete and accurate
- [ ] Retrieved date is correct (YYYY-MM-DD format)
- [ ] Citation is correct
- [ ] Source type noted
- [ ] Any important notes added

### File Organization
- [ ] File saved in correct subdirectory
- [ ] File named per naming convention
- [ ] PDF downloaded and saved (if available)
- [ ] PDF in correct binary_files/ subdirectory

### Formatting
- [ ] Metadata header at top of file
- [ ] Separator line (`---`) between header and text
- [ ] Text is readable (no major formatting issues)

---

## Organizing Existing Files

Some sources already have raw files that just need organization.

### Sources with Existing Files

1. **Regulation X** - PDF and raw.md exist
2. **Regulation Z** - PDF and raw.md exist  
3. **NAR Code of Ethics 2025** - PDF and raw.md exist

### Process for Existing Files

**Step 1: Locate Existing Files**
- See ASSIGNMENTS.md for file locations
- Example: NAR files in `/Users/go/.../Content Audit/NAR-Code-of-Ethics/`

**Step 2: Review Files**
- Open existing raw.md file
- Open existing PDF file
- Verify completeness and accuracy

**Step 3: Add/Update Metadata Header**
- Check if metadata header exists
- If not, add using template above
- If exists, verify all fields are complete

**Step 4: Copy to Raw_Source_Collection**
- Copy .md file to appropriate subdirectory in Raw_Source_Collection/
- Example: NAR → `professional_standards/nar_code_of_ethics_2025_raw.md`

**Step 5: Move PDF to binary_files/**
- Move PDF to appropriate binary_files/ subdirectory
- Example: NAR PDF → `binary_files/professional_standards/NAR_Code_of_Ethics_2025.pdf`

**Step 6: Verify Against Official Source**
- Visit official URL
- Compare existing file to current official version
- Note if any updates needed

**Step 7: Mark Complete**
- Update checklist in ASSIGNMENTS.md

---

## Common Issues & Solutions

### Issue 1: Website Requires Navigation Through Multiple Pages

**Solution:**
- Use "Print View" or "Download" features if available
- Copy each page systematically
- Verify completeness using table of contents

### Issue 2: Copy/Paste Formatting Issues

**Solution:**
- Paste into plain text editor first
- Clean up excessive line breaks
- Keep section structure intact
- Don't worry about perfect formatting - raw is okay

### Issue 3: Can't Find Official PDF

**Solution:**
- Many statutes don't have official PDFs
- This is okay - the text version is primary
- Note in metadata: "No official PDF available"

### Issue 4: Uncertain if Text is Complete

**Solution:**
- Check for section numbering gaps
- Compare to table of contents on official site
- Look for "end of chapter" or similar indicators
- Ask for review if uncertain

### Issue 5: Virginia LIS Site Navigation

**Solution:**
- Virginia LIS can be tricky to navigate
- Use "Whole Chapter" view when available
- Cross-reference with section lists
- Alternative: Use law.lis.virginia.gov search function

### Issue 6: Updates or Amendments

**Solution:**
- Always use current version on official site
- Note date in metadata ("as of [date]")
- If site shows "current through [date]", note this
- Don't worry about historical versions

---

## Tips for Efficiency

1. **Start with High Priority** - Verified sources first (Fair Housing, RESPA, NAR)
2. **Batch Similar Sources** - Do all federal statutes together, then regulations, then Virginia
3. **Use Browser Tools** - Reader mode, print view, developer tools to select text
4. **Save Often** - Don't lose work to browser crashes
5. **Verify as You Go** - Easier to catch errors immediately
6. **Document Questions** - Note anything unclear in metadata for review

---

## Estimated Time Per Source

- **Federal Statutes (short):** 20-30 minutes (ECOA, Lead Paint)
- **Federal Statutes (medium):** 30-45 minutes (Fair Housing, TILA)
- **Federal Statutes (long):** 45-60 minutes (RESPA, FCRA)
- **Federal Regulations:** 30-45 minutes (Regulation X, Z)
- **Virginia Statutes:** 30-45 minutes each
- **Virginia Regulations:** 30-45 minutes
- **NAR Code of Ethics:** 15-20 minutes (organizing existing)
- **Organizing Existing Files:** 10-20 minutes each

**Total Estimated Time: 6-14 hours** (spread over days/weeks)

---

## Getting Help

**Questions or Issues:**
- Document in ASSIGNMENTS.md notes section for specific source
- Create request file in Team/Sourabh Manager/ if needed
- Continue with other sources while waiting for clarification

**Technical Issues:**
- Browser not copying text correctly → Try different browser
- Website down → Note in ASSIGNMENTS.md, move to next source
- File won't save → Check file path and permissions

---

## Final Checklist Before Marking Complete

For each source:
- [ ] Raw text collected from official URL
- [ ] Metadata header complete with all required fields
- [ ] File saved with correct naming convention in correct subdirectory
- [ ] PDF downloaded (if available) and saved to binary_files/
- [ ] Self-verified for completeness and accuracy
- [ ] Checklist items in ASSIGNMENTS.md marked complete
- [ ] Ready for review

---

**Remember:** Quality over speed. It's better to take extra time to ensure accuracy than to rush and need corrections later.

**Last Updated:** 2025-11-13  
**Version:** 1.0
