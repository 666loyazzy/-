# Strict Edge-Cloud LLM 20-Paper Curation Implementation Plan

> **For agentic workers:** Execute every checkbox in order and do not weaken the strict edge-cloud inclusion rule to fill the quota.

**Goal:** Replace every non-qualifying entry while retaining DynO, DynoPipe, and PrivacyAware, leaving exactly 20 strict edge/device-cloud collaborative LLM inference papers with original, Chinese mono, and bilingual dual PDFs.

**Architecture:** Treat the repository index as the source of truth. A paper qualifies only when endpoint/edge and cloud/server jointly contribute to the same inference result. Rank qualifying work by venue tier, obtain legal open copies, translate with pdf2zh and AI terminology, then verify PDF structure and every rendered page before publishing.

**Tech Stack:** Git, pdf2zh/PDFMathTranslate, Poppler, PyMuPDF, pypdf, pdffonts.

**Spec:** User requires exactly 20 papers, retains DynO/DynoPipe/PrivacyAware, prioritizes top conferences, and requires embedded-text Chinese translations without omissions, font corruption, or rendering failures.

## Global Constraints

- [ ] Exactly 20 originals and 40 translated PDFs at completion.
- [ ] Keep DynO, DynoPipe, and PrivacyAware.
- [ ] Reject pure-device, pure-cloud, generic serving, surveys, and legacy CNN/DNN split inference.
- [ ] Prefer ISCA/MICRO/HPCA/ASPLOS, then EuroSys/MobiSys/MobiCom/INFOCOM/ACL/UCC/ICC/SoCC.
- [ ] Require open original PDF provenance and record official venue/DOI metadata.
- [ ] Use consistent AI terminology; reject mistranslations such as `法学硕士` for LLM.

## Task 1: Freeze the 20-paper inclusion matrix

- [ ] Classify all current entries against the strict rule.
- [ ] Select ten formal-venue replacements for the ten removals.
- [ ] Record one-sentence collaboration evidence and venue evidence for every entry.

## Task 2: Replace source PDFs

- [ ] Download ten open author, arXiv, or anthology PDFs into `papers/original/`.
- [ ] Validate `%PDF`, page count, title text, and non-truncated downloads.
- [ ] Remove the ten rejected originals and their translations.

## Task 3: Translate with pdf2zh

- [ ] Generate `-mono.pdf` and `-dual.pdf` for every new paper.
- [ ] Apply the terminology glossary for edge-cloud collaborative LLM inference.
- [ ] Preserve equations, figures, tables, citations, and page geometry.

## Task 4: PDF quality assurance

- [ ] Match original/mono/dual page counts for all 20 papers.
- [ ] Verify extractable Chinese text and embedded CJK fonts.
- [ ] Scan for untranslated body text, forbidden mistranslations, missing glyphs, and empty pages.
- [ ] Render every translated page and reject Poppler/font/render errors.
- [ ] Visually inspect representative dense text, equation, table, figure, and reference pages.

## Task 5: Update and publish repository metadata

- [ ] Update `README.md`, `PAPERS.md`, `TAXONOMY.md`, and paper README files.
- [ ] Update `papers/SOURCES.tsv` and `papers/QA_REPORT.md` from measured results.
- [ ] Confirm repository counts and zero stale filenames.
- [ ] Commit, push `edge-cloud-papers`, and verify the remote branch SHA and tree.
