---
title: "Intrusion Alert Explainer"
subtitle: "Mapping IDS/Snort alerts to CVE vulnerabilities with ranked retrieval"
excerpt: "A cybersecurity tool that maps IDS and Snort alerts to CVE vulnerabilities using TF-IDF ranked retrieval, CVSS severity scoring, and CWE-based remediation guidance across 43,000+ NVD entries."
date: 2026-04-01
author: "Germaine Hounakey"
draft: false
tags:
  - python
  - cybersecurity
  - nlp
categories:
  - Projects
layout: single
---

## Overview

Intrusion Alert Explainer is a Python-based cybersecurity tool that takes raw IDS and Snort alerts and maps them to known CVE vulnerabilities — turning a cryptic alert into an explainable, prioritized finding.

## How it works

- Uses **TF-IDF ranked retrieval** to match alert text against a database of **43,000+ NVD vulnerability entries**.
- Scores matches with **CVSS severity ratings** so the most critical issues surface first.
- Attaches **CWE-based remediation guidance** to each match, giving analysts a concrete next step rather than just a vulnerability ID.

## Stack

Python, TF-IDF / scikit-learn style retrieval, CVE / CVSS / CWE data sources.

[View the repository →](https://github.com/shahedadel/CVE_Threat_Intelligence_Analysis_System)
