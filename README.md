# DS‑Conv1D Benchmarks

This repository contains experiments comparing the Domain‑Specific 1D convolution (DS‑Conv1D) architecture used in the EdgeSense‑1W project against standard 1D convolution and other lightweight models on vibration condition‑monitoring datasets such as the Case Western Reserve University (CWRU) bearing dataset.

The goal is to evaluate whether DS‑Conv1D can achieve comparable classification accuracy while significantly reducing multiply‑accumulate operations and power consumption.

## Datasets

* **CWRU bearing dataset** – publicly available dataset for bearing fault diagnosis.
* Additional public vibration datasets can be added via pull requests.

## Models compared

* **DS‑Conv1D** – depthwise‑separable convolutional network tailored for vibration signals.
* **Standard Conv1D** – baseline 1D CNN architecture.
* **Other lightweight models** – e.g., BGRU, Transformer variants (optional).

## Usage

1. Install Python dependencies from `requirements.txt`.
2. Run `python train.py --model dsconv1d --dataset cwru` to train DS‑Conv1D.
3. Evaluate using `python evaluate.py`.

Detailed instructions and code will be added as the benchmark suite evolves.

## Status

This benchmark suite is under development. Contributions and suggestions for additional datasets or models are welcome.
