# GPT Sketchpad

Collection of Jupyter Notebooks building up to reproduce GPT-2 from scratch.

## Setup

```
git clone git@github.com:marcinbogdanski/zerotohero-repro.git
cd zerotohero-repro
uv sync
```

Notebooks in `notebooks` should be runnable now.

## GPT-2 Reproduction

Prepare data with:

- `letsbuildgpt/fineweb.ipynb`
- `letsbuildgpt/hellaswag.ipynb`.

Then run training with:

```bash
uv run torchrun --standalone --nproc_per_node=2 letsbuildgpt/train_gpt2.py
```
