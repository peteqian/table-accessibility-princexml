# PrinceXML Table Accessibility Reproduction

## Overview

This repository serves as a minimal reproduction of an accessibility issue encountered when generating PDFs from HTML tables using **PrinceXML**. Specifically, the problem involves screen readers (e.g., VoiceOver on macOS) misinterpreting table semantics in the resulting PDF, despite the HTML table being correctly structured and accessible in the browser.

- **minimal.html**: The HTML file containing the table structure that reproduces the accessibility issue.
- **output.pdf**: The resulting PDF file generated from `minimal.html` (included for reference).

When converting the provided HTML table to PDF using PrinceXML with the following command:

```bash
prince minimal.html --structured-log=buffered --javascript --output=output.pdf --pdf-profile=PDF/A-3a+PDF/UA-1
```
