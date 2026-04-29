---
layout: page
title: TRACK
description: An Open-Source, Global Trace Library for Trace-Based Simulators
img: assets/img/library-oslo.jpg
importance: 1
category: data-management
related_publications: true
---

This decentralized trace repository project is designated the **T**race **R**epository for **A**rchitecture & **C**omputation **K**nowledge, hence the acronym **TRACK**.

## Table of Contents
- [About the Project](#about-the-project)
- [Project Structure](#project-structure)
- [Contribution](#contribution)
- [License](#license)
- [Authors](#authors)
- [Citing](#citing)

## About the Project

Over the past decade, the volume of micro-architecture research leveraging the [ChampSim Simulator](https://champsim.github.io/ChampSim/) has grown exponentially. While ChampSim has been instrumental in driving significant innovations within the community, its underlying infrastructure has suffered from a critical bottleneck: the lack of standardized, accessible trace repositories. This scarcity severely impedes the reproducibility of results presented in recent literature.

My own research has not been immune to this challenge; accessing the precise trace sets required to validate prior work has proven increasingly difficult (*c.f.*, {% cite jamet_characterization_iiswc_2020 jamet_tlp_hpca_2024 jamet_sdc_ipdps_2024 jamet_ip_cat_isca_2026 %}). To address this, the TRACK project proposes a **FAIR** approach to trace management. In the context of scientific research, FAIR is an acronym for the four core principles defined by the [GO FAIR Initiative](https://www.go-fair.org/):

- **<u>F</u>indable**: The primary step in (re)using data is its discovery. Metadata and data must be easily discoverable by both humans and machines. Machine-readable metadata are essential for the automatic discovery of datasets, serving as a foundational component of the FAIRification process.
- **<u>A</u>ccessible**: Once the required data are located, users must know how to access them, including any necessary authentication or authorization protocols.
- **<u>I</u>nteroperable**: Data typically need to be integrated with other datasets. Furthermore, they must be capable of interoperating with diverse applications, workflows, and processing environments.
- **<u>R</u>eusable**: The ultimate goal of FAIR is to optimize data reuse. To achieve this, metadata and data must be richly described with clear provenance and usage licenses, enabling them to be replicated or combined in different experimental settings.

Specifically, the TRACK project is designed to deliver two core components:

1.  **A Unified Metadata Standard for Software Traces**: We define a common schema for trace metadata compatible with trace-based simulators, including [ChampSim](https://champsim.github.io/ChampSim/) and [ZSim](https://github.com/s5z/zsim). This standard ensures the consistent description and organization of trace data across diverse simulation environments.
2.  **A Streamlined Command-Line Interface (CLI)**: We provide a robust and intuitive CLI to simplify user interaction with the trace registry. This tool enables efficient querying, retrieval, and management of traces, lowering the barrier to entry for researchers and facilitating reproducible workflows.

## Project Structure

In an effort to address the aforementioned limitations of the current trace-based simulation pipeline, this project provides two main components distributed across two repositories:

1.  The **[TRACK Schema](https://github.com/jesuisalexjamet/track-schema)** repository, which defines the standard governing the operation of the trace registry.
2.  A forthcoming repository containing a **Command-Line Interface (CLI)** designed to simplify interaction with the trace registry.

## Contribution

Contributions are welcome. Please refer to the repository guidelines. (Work in Progress) :smile:

## License

This project is licensed under the Academic Free License ("AFL") v3.0. See [AFL v3.0 on SPDX](https://spdx.org/licenses/AFL-3.0.html) for details.

## Authors

- **Alexandre V. Jamet** -- <alexandre.jamet@bsc.es>

## Citing

Citation guidelines are currently being prepared. (Work in Progress) :smile: