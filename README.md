# CorA-XML scripts

This repo contains scripts mainly to process files from the [Anselm Corpus](https://www.linguistics.rub.de/anselm/), which are provided in CorA-XML format.

While there is [documentation for the CorA-XML file format](https://cora.readthedocs.io/en/latest/coraxml/) and some helper scripts are [provided as part of the CorA repository](https://github.com/comphist/cora/tree/master/bin), the XML files of the Anselm Corpus that are [offered for download](https://www.linguistics.rub.de/anselm/access/index.en.html) do not follow this format exactly, so the scripts will fail to work.

## Usage

All scripts provide the `-h`/`--help` switch with detailed information.

### Extract tokens and annotations

Probably the most common use case.

Extract tokens in UTF representation with their normalization:

```bash
$ ./extract_coraxml.py FILENAME -f utf -t norm
```

Extract tokens in simplified representation with POS and morphology tags:

```bash
$ ./extract_coraxml.py FILENAME -f ascii -t pos morph
```
