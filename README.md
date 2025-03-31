# EFICaS

EFICaS (Elementary Fuzzy Inference Control at Scale), a control protocol that leverages the monitors' semantic understanding by prompting them to output fuzzy semantic labels instead of a non-deterministic numeric suspicion score to build a transparent, explainable control protocol with low latency and low cost.

## Prerequisites

Ensure you have [uv](https://docs.astral.sh/uv) installed

## Installation

Clone the repository

```
git clone --recurse-submodules git@github.com:jplv-challenges/EFICaS.git
cd EFICaS
```

Create the Python environment with uv

```
uv sync
```

## Usage

### Examples

Make sure to fill in your API keys inside *control-arena/.env*

```
uv run --env-file control-arena/.env control-arena/examples/evals/monitors_llm_bash.py --limit 10 --cache_honest False --cache_attack False 
```