---
name: flow-diagram
description: Build or check a participant or study flow diagram (CONSORT, PRISMA, STROBE, STARD) in LaTeX from the numbers the authors provide.
---

Use this when a manuscript needs a flow diagram, or has one whose numbers need checking.

1. Establish which diagram: trial participant flow (CONSORT), records and studies in a review (PRISMA), participants in an observational study (STROBE) or in a diagnostic accuracy study (STARD). Ask for the guideline version and any extension, because the official diagram differs between them (a cluster trial tracks clusters as well as participants; a review update or a search of registers and other sources has extra columns).
2. Obtain the official template or its description from the collaborator or from the guideline's website or the EQUATOR Network (www.equator-network.org) with fetch_url, and follow its boxes and their order. Do not lay the diagram out from memory. Where the guideline asks for a flow diagram without publishing a template (STROBE does this), say so, obtain the official checklist text the same way (ask the collaborator for the file if it cannot be fetched), and build the boxes from the stages its item on participants names, in that order, confirming the stages with the collaborator.
3. Collect the numbers. Take them from the manuscript text and tables where they are stated, and ask the collaborator for every one that is not. Never fill a box with a number you derived by assuming the others are right, and never invent a reason for exclusion; a derived number is shown to the collaborator as derived and confirmed before it goes in.
4. Check the arithmetic before drawing, and report every mismatch with the two figures that disagree:
   - each stage equals the stage before minus what left at that step;
   - reasons for exclusion sum to the number excluded at that step;
   - arms sum to the number randomised or enrolled;
   - for each arm: allocated, received, lost, discontinued and analysed are consistent, and anyone excluded from analysis has a reason;
   - for a review: records per source sum to the total identified; after duplicates, screened, sought, not retrieved, assessed and included follow from one another; studies and reports are counted separately where they differ;
   - the final numbers equal the denominators in the results tables.
   Stop and ask when the numbers cannot be reconciled; do not adjust one to make the diagram close.
5. Draw it in the project's own way. If the project already has a diagram, edit it. Otherwise use TikZ with nodes of fixed text width placed relative to one another (the positioning library), one style for boxes and one for arrows, exclusions set to the side of the main column, and arms side by side. Keep the numbers in the node text in a consistent form, n = 123, with reasons listed under the count. Load only packages the class allows, and prefer a standalone figure file that the manuscript includes.
6. Keep the wording of each box as the template has it, adapted only where the template says to adapt it; without a template, use the checklist's own terms for each stage.
7. Compile and look at the result with read_pdf: nothing overlapping, no text cut off, readable at the journal's column width, arrows meeting the boxes. Fix and recompile.
8. Add a caption, a label, and a reference to the figure in the text where participants or study selection are described, if there is none.
9. Report the numbers used and where each came from (manuscript location, or the collaborator), the mismatches found, and any box left with a marked placeholder.
