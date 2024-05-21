# GKS-ClinVar

<!-- [![image](https://img.shields.io/pypi/v/gks-clinvar.svg)](https://pypi.python.org/pypi/gks-clinvar)
[![image](https://img.shields.io/pypi/l/gks-clinvar.svg)](https://pypi.python.org/pypi/gks-clinvar)
[![image](https://img.shields.io/pypi/pyversions/gks-clinvar.svg)](https://pypi.python.org/pypi/gks-clinvar)
[![Actions status](https://github.com/ga4gh/gks-clinvar/actions/workflows/checks.yaml/badge.svg)](https://github.com/ga4gh/gks-clinvar/actions/checks.yaml) -->

A submission tool for submitting to the ClinVar Submission API using [GA4GH Genomic
Knowledge Standards](https://www.ga4gh.org/work_stream/genomic-knowledge-standards/)
(GKS) data.

Development of a shared, open-source software package for managing these submissions
that can be easily configured for use by multiple submitters would be highly impactful
as development and adoption of the GKS framework grows.

![image](./misc/images/GKS-ClinVar%20submission%20overview.png)

We plan to contribute to [ClinVar This](https://github.com/varfish-org/clinvar-this) to
support GKS data stored as [JSON Lines](https://jsonlines.org/) files.

---

## ClinVar Submission API

* Documentation: <https://www.ncbi.nlm.nih.gov/clinvar/docs/api_http/>
* GitHub: <https://github.com/ncbi/clinvar/tree/master/submission_api_schema>

### ClinVar Submission API Analysis

The [analysis](./analysis/) directory contains example CIViC and VarCat submissions to the [test Submission API](https://submit.ncbi.nlm.nih.gov/apitest/v1/submissions). This analysis focused on submitting `oncogenicitySubmission` and `clinicalImpactSubmission` objects.

<!-- ## Installation

Install from [PyPI](https://pypi.org/project/gks-clinvar/):

```shell
python3 -m pip install gks-clinvar
``` -->

---

## Development

Clone the repo and create a virtual environment:

```shell
git clone https://github.com/ga4gh/gks-clinvar
cd gks-clinvar
python3 -m virtualenv venv
source venv/bin/activate
```

Install development dependencies and `pre-commit`:

```shell
python3 -m pip install -e '.[dev,tests,analysis]'
pre-commit install
```

Check style with `ruff`:

```shell
python3 -m ruff format && python3 -m ruff check --fix
```

<!-- Run tests with `pytest`:

```shell
pytest
``` -->
