# Red Light Detection Technical Report

**Educational project documentation · Russian · PDF**

A technical report documenting an educational application for analyzing traffic photographs and videos. It brings together the problem statement, requirements, system design, processing algorithms, API overview, installation instructions, and a testing section.

## My contribution

I wrote the report, formatted it, edited the text, and made corrections throughout the document.

## Intended readers

The report supports academic review of the project and gives technical readers an overview of the system. Its API and installation appendices address readers who want to explore the application. This audience description is based on the report's structure and contents.

## Documentation scope

- Functional requirements with identifiers FR-01 through FR-08 and acceptance criteria.
- Architecture and a file-processing sequence illustrated with diagrams.
- Descriptions of vehicle detection, tracking, traffic-light classification, and stop-line handling.
- Data storage, API routes, result export, and launch options.
- A multipart request example and a JSON response example.
- Installation and usage instructions.

## Technologies described

Python, FastAPI, OpenCV, YOLOv8n in ONNX format, ONNX Runtime, SQLite, PyWebView, ReportLab, and openpyxl. These are technologies described in the report, not a claim of independently verified proficiency in every tool.

## Suggested reading

| Topic | Section | Printed pages |
|---|---|---|
| Requirements and acceptance criteria | 2.1 | 9–10 |
| Architecture and processing flow | 2.3 | 11–12 |
| API route overview | 3.1 | 19 |
| Request and response examples | Appendix A | 26 |
| Installation and usage | Appendix B | 27 |

The supplied PDF begins with the contents page numbered 2. Its PDF page index therefore differs from its printed page number.

## What this sample demonstrates

Structuring a substantial technical report, connecting requirements to implementation descriptions, explaining a processing workflow, and combining narrative text with tables, diagrams, and API examples.

## Review status

This is the supplied report, with its original contents preserved. Some descriptions of photo-analysis status, stop-line fallback behavior, and processing time differ between sections and need reconciliation before a revised edition is presented as authoritative. The portfolio does not repeat those values as verified implementation results.

[Read the supplied report](../downloads/red-light-detection-report.pdf)

**Source:** supplied “Отчет.pdf”, sections 2–3 and appendices A–B. My contribution is described as confirmed by me for this portfolio. Software behavior and testing outcomes have not been independently reproduced during the document review.
