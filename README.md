# Web Research & Citation Fact-Checker

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Stack: Python & BeautifulSoup](https://img.shields.io/badge/Stack-Python%20%7C%20BeautifulSoup4-brightgreen.svg)]()
[![Focus: Hallucination Detection](https://img.shields.io/badge/Task-Citation%20Grounding-red.svg)]()

**Author:** Jacob Astorga  
**Focus:** Automated pipeline validating AI-generated claims and URLs against live web sources to detect broken links and hallucinated citations.

---

## 📌 Overview

`web-citation-fact-checker` is an automated fact-checking and grounding verification tool designed for evaluating AI search agents, automated research assistants, and LLM text generation pipelines.

### Key Capabilities
* **Automated URL Extraction & Liveness Verification:** Parses Markdown/HTML text, identifies all cited endpoints, and executes parallel HTTP HEAD/GET probes to detect dead links (404s, SSL errors, redirect loops).
* **DOM Content Parsing:** Uses `BeautifulSoup4` to extract clean page text, meta tags, and structured headers, discarding boilerplate and paywall banners.
* **Semantic Grounding Verification:** Cross-references key technical claims and numbers against parsed live source content to detect subtle hallucinated attributions.

---

## 🚀 Quick Start

```bash
git clone https://github.com/jacobastorga/web-citation-fact-checker.git
cd web-citation-fact-checker
python src/citation_checker.py
```

---

## 📄 License
MIT License - see [LICENSE](LICENSE) for details.
