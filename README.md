# Archived implementation: PDF extraction

The maintained implementation is [zixcel-document-output](https://github.com/zixcel/zixcel-document-output). Use its Rust `pdf-analyze` command for text extraction, metadata, page analysis, and JSON reports. Read and report-write permissions are authorized separately.

This repository preserves the original Python implementation, issues, pull requests, and commit history for reference. The maintained package README defines input digest requirements, zero-based page selection, and output permissions. Synthetic comparison fixtures verified extracted text after whitespace normalization and decoded metadata. The Rust implementation also corrects nested-image detection and image-only counters. No customer PDFs are included.

## Legacy structure

`src/pdf2text/` contains extraction and metadata analysis. `src/workflow/` and `src/cli/` contain the historical command integration. `docs/` and locale files are historical documentation. New callers should use the maintained Rust package interface. No consumers outside this legacy package were found in the inspected workspace source roots.

## License

Apache-2.0 applies to the maintained repository source. See LICENSE and NOTICE; preserve third-party dependency and translation attributions. Local registration inputs and generated reports are excluded from source publication.
