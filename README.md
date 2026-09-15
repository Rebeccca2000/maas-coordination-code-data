# Coordination architecture comparison code and data

This repository contains the code and numerical data for the accompanying Nature Communications manuscript comparing centralised and decentralised Mobility as a Service coordination. Manuscript files and submitted figures are excluded.

## Authors

- [Ruiyi Zhao](https://edas.info/showPerson.php?p=2467850&c=34965), University of New South Wales, Australia
- [Khaled Almiani](https://edas.info/showPerson.php?p=1664449&c=34965), Higher Colleges of Technology, United Arab Emirates
- [Salil S Kanhere](https://edas.info/showPerson.php?p=108880&c=34965), UNSW Sydney, Australia
- [Travis Waller](https://edas.info/showPerson.php?p=132851&c=34965), The University of Texas at Austin, USA
- [Taha H. Rashidi](https://edas.info/showPerson.php?p=2026639&c=34965), University of New South Wales, Australia

## Download and verification

Download `maas-coordination-code-data.zip` from this repository. The archive contains the model code, paired experiment runners, 46 frozen input worlds, request-level outputs for the stress and sensitivity experiments, final numerical source data, licences and a SHA-256 manifest.

Archive SHA-256: `76bf2d9d25bdd1d6d7e53c498afb2f0296d534a1c3f5f2c6bd4dd8e1ff60ee9c`

After extracting the archive, reproduce the five headline stress metrics with:

```bash
python code/analysis/reproduce_headline_metrics.py --check
```

A successful check reproduces all 40 rows in the archived five-metric source table.

## License

The code is released under the MIT License. Data are released under the Creative Commons Attribution 4.0 International License. The full terms are included in the archive.
