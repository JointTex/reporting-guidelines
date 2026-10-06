# Reporting guidelines

Find the reporting guideline a study needs, check the manuscript against its official checklist item by item, and build the flow diagram.

A JointTex skill set. Publish this repository from the JointTex plugin marketplace (Plugins, Publish skills) with the values below; each skill is `skills/<name>/SKILL.md`.

- Name: Reporting guidelines (zh: 报告规范)
- Summary: Pick the right reporting guideline and check a manuscript against CONSORT, SPIRIT, PRISMA, STROBE, STARD, TRIPOD, CARE, ARRIVE, SRQR or COREQ, or any checklist you supply.
- Summary (zh): 选定适用的报告规范，并按 CONSORT、SPIRIT、PRISMA、STROBE、STARD、TRIPOD、CARE、ARRIVE、SRQR、COREQ 或你提供的任意清单逐条检查稿件。
- Fields: medicine, life-sciences, writing

## Skills

Start here when the design or the guideline is not settled:

- `guideline-select`: Work out which reporting guideline and extensions apply to a study from its design, and where to get the official checklist.

One check per study type:

| Skill | Study | Guideline |
| --- | --- | --- |
| `consort-check` | randomised trial | CONSORT |
| `spirit-check` | clinical trial protocol | SPIRIT |
| `prisma-check` | systematic review or meta-analysis | PRISMA |
| `strobe-check` | cohort, case-control or cross-sectional study | STROBE |
| `stard-check` | diagnostic accuracy study | STARD |
| `tripod-check` | prediction model development or validation | TRIPOD |
| `care-check` | case report | CARE |
| `arrive-check` | animal research | ARRIVE |
| `qualitative-check` | qualitative research | SRQR or COREQ |
| `checklist-check` | anything else | any checklist you supply (CHEERS, SQUIRE, TREND, a journal's own form) |

And for the figure most of them ask for:

- `flow-diagram`: Build or check a participant or study flow diagram (CONSORT, PRISMA, STROBE, STARD) in LaTeX from the numbers the authors provide.

## How a check works

Every check follows the same steps: obtain the official checklist text (a file you add to the project, or fetched from the guideline's website or the EQUATOR Network), read the whole manuscript with its supplement, record each item as reported, partly reported, not reported or not applicable with its location and a short quotation, cross-check the numbers between text, tables and figures, and hand back the completed checklist table with a prioritised list of gaps.

## What the skills will not do

They do not work from a remembered checklist: items and their numbering differ between versions and extensions, so a check stops and asks for the file when the official text cannot be obtained. They assess what the manuscript reports, not how well the study was conducted, and they are not a risk-of-bias assessment. They never fill a gap with invented study details (registration numbers, sample size calculations, counts, dates, approvals); missing information is asked for and left as a marked placeholder.

The checklists themselves belong to their guideline groups and are not copied into this repository.

## License

MIT. See [LICENSE](LICENSE).
