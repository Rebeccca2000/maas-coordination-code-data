# Coordination architecture comparison: code and data

This repository contains the code and numerical data supporting the accompanying
Transportation Research Part C manuscript:

**A controlled agent-based comparison of centralised dispatch and decentralised
mobility markets reveals cost, coverage and time-equity trade-offs**

The repository contains the model code, experiment runners, frozen input worlds,
request-level outputs, numerical source data, licences and verification files.
Manuscript files and submitted figures are excluded from this repository.

## Authors

- Ruiyi Zhao — Research Centre for Integrated Transport Innovation (rCITI),
  UNSW Sydney, Australia
- Taha H. Rashidi — Research Centre for Integrated Transport Innovation (rCITI),
  UNSW Sydney, Australia
- Khaled Almi’ani — Higher Colleges of Technology, United Arab Emirates
- Salil S. Kanhere — UNSW Sydney, Australia
- S. Travis Waller — TU Dresden, Germany

## Download and verification

Download `maas-coordination-code-data.zip` from this repository and extract it
before running the verification command.

The archive contains:

- model and analysis code;
- paired centralised and decentralised experiment runners;
- 46 frozen input worlds;
- request-level outputs for the stress and sensitivity experiments;
- final numerical source data;
- licence files; and
- a SHA-256 manifest.

Archive SHA-256:

```text
76bf2d9d25bdd1d6d7e53c498afb2f0296d534a1c3f5f2c6bd4dd8e1ff60ee9c
```

From the extracted archive, reproduce the five headline stress metrics with:

```bash
python code/analysis/reproduce_headline_metrics.py --check
```

A successful check reproduces all 40 rows in the archived five-metric source table. The model is designed as a lightweight, mechanism-focused agent-based test bed.
It compares coordination architectures under controlled shared inputs; it is not intended to provide a full population-representative forecast of Sydney.

## License

The code is released under the MIT License. Data are released under the Creative Commons Attribution 4.0 International License. The full terms are included in the archive.
