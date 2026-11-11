<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img src="assets/banner-light.svg" alt="Carbon Research Labs: open-source software, measured, not claimed. Carbon-OCR, Fullerene, fullerene-data and Standard Quant Tools." width="100%">
</picture>

<p>
  <a href="https://github.com/CarbonResearchLabs/Carbon-OCR"><img alt="Carbon-OCR: C++ and CUDA" src="https://img.shields.io/badge/Carbon--OCR-C%2B%2B%20and%20CUDA-5bbff4?style=flat-square&labelColor=1a1a1a"></a>
  <a href="https://huggingface.co/CarbonResearchLabs/fullerene-3M"><img alt="models: fullerene-3M on Hugging Face" src="https://img.shields.io/badge/models-fullerene--3M-74f2d6?style=flat-square&labelColor=1a1a1a"></a>
  <a href="https://huggingface.co/datasets/CarbonResearchLabs/fullerene-data"><img alt="data: fullerene-data" src="https://img.shields.io/badge/data-fullerene--data-79ee5f?style=flat-square&labelColor=1a1a1a"></a>
  <a href="https://github.com/CarbonResearchLabs/Standard-Tools"><img alt="Standard Quant Tools: Python, C++ core" src="https://img.shields.io/badge/Standard%20Quant%20Tools-Python%2C%20C%2B%2B%20core-f2b43c?style=flat-square&labelColor=1a1a1a"></a>
  <img alt="code: Apache 2.0" src="https://img.shields.io/badge/code-Apache%202.0-d6352a?style=flat-square&labelColor=1a1a1a">
</p>

**Carbon Research Labs builds open-source software in which every number is measured, never estimated.** Two
projects are public: Carbon-OCR, an OCR engine in C++ and CUDA with its own family of small models, Fullerene; and
Standard Quant Tools, a Python library for quantitative finance, built to be called by AI agents.

## <img src="assets/chip-01.svg" height="22" alt=""> Carbon-OCR and Fullerene

[**Carbon-OCR**](https://github.com/CarbonResearchLabs/Carbon-OCR) reads scans, photos of documents and PDFs into text,
markdown, HTML and JSON with boxes, in reading order, with labeled blocks and table cells. It runs on CPUs, with its
own int8 kernels or with ONNX Runtime, one worker per core, and on NVIDIA GPUs through TensorRT, with many pages in
flight. It also writes hOCR, ALTO, PAGE XML and searchable PDF.

[**fullerene-3M**](https://huggingface.co/CarbonResearchLabs/fullerene-3M) is its Latin model set, for Latin, Cyrillic
and Greek: four networks with 2.77 M parameters in all, trained from scratch, for page orientation, line detection,
line recognition, and reading order with block labels and table cells. Read by Carbon-OCR, it scores a headline of
**44.5** on all 2,937 pages of OmniParseBench, where Tesseract 5.5 scores 5.9.

[**fullerene-data**](https://huggingface.co/datasets/CarbonResearchLabs/fullerene-data) records the training data
source by source: where each came from, its license, and every file's checksum.

## <img src="assets/chip-02.svg" height="22" alt=""> Standard Quant Tools

[**Standard Quant Tools**](https://github.com/CarbonResearchLabs/Standard-Tools) is a Python library for quantitative
finance, built to be called by AI agents. Every tool takes one Pydantic model and returns one, so an agent gets
structured data back, and errors that say what to fix. Its 266 tools are split across twelve runtimes, and a client
is served one runtime at a time, over MCP or as function-calling schemas. The CPU-bound paths run in an optional C++
extension behind the same API, with a pure-Python fallback.

## <img src="assets/chip-03.svg" height="22" alt=""> Licenses

- Carbon-OCR and Standard Quant Tools: Apache 2.0.
- The Fullerene weights: the [Carbon-OCR OpenRAIL-AMS](https://huggingface.co/CarbonResearchLabs/fullerene-3M/blob/main/LICENSE-WEIGHTS.md),
  royalty-free under its use restrictions.

<sub>[getcarbonresearch.com](https://getcarbonresearch.com) · [huggingface.co/CarbonResearchLabs](https://huggingface.co/CarbonResearchLabs)</sub>
