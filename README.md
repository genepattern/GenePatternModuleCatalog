# GenePattern Module Catalog

An open-source archive of [GenePattern](https://www.genepattern.org) module zip files, preserved to support reproducible computational biology research.

## Purpose

GenePattern is a genomic analysis platform, initiallyy developed at the Broad Institute with continued development at the University of California San Diego, that provides access to hundreds of bioinformatics tools through a common interface. This repository is a copy of the GenePattern public module catalog server, archiving the module zip files that make up that catalog.

By hosting these artifacts publicly, this repository ensures that analyses performed with GenePattern modules can be reproduced in the future  if the original module server is unavailable,  preserving the provenance chain for published research.

## Contents

The repository contains ~ **265 modules** aorganized as follows:

```
modules/
  <ModuleName>/
    <lsid-authority:lsid-namespace>/
      <lsid-id>/
        <version>/
          <ModuleName>.zip
suites/
  <SuiteName>/
    ...
```

Each module may have multiple versioned zip files, corresponding to the published versions available on the GenePattern module repository.

## Usage

To get a module zip file:

1. Browse to the module directory of interest under `modules/`
2. Select the desired version
3. Download or reference the `.zip` file directly

The zip files are in standard GenePattern module format and can be used in several ways:

- **GenePattern Server** — Install on any GenePattern server via the "install Module" menu item on the "Modules & Pipelines" menu or the GenePattern API. To run your own server, see [genepattern/genepattern-server](https://github.com/genepattern/genepattern-server).
- **Local Docker execution** — Run modules locally from their zip files using Docker, without a full server installation, via the [GenePattern Local Runner MCP](https://github.com/genepattern/local_genepattern_runner_mcp).

## About GenePattern

GenePattern provides hundreds of analytical tools for gene expression analysis, proteomics, SNP analysis, flow cytometry, RNA-seq, and more. Source code for many of the modules are available in the [GenePattern github organization](https://github.com/genepattern/).

## License

Module zip files are subject to their individual licenses as specified within each module. This archive is provided for reproducibility and research continuity purposes.
