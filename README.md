## Direct Imitation Learning: RLHF Secretly Performs Imitation Learning

This repository contains the code for the ICLR 2025 submission [Direct Imitation Learning: RLHF Secretly Performs Imitation Learning](https://openreview.net/forum?id=2QdsjiNXgj). 


### Environment

First, install PyTorch `2.1.2` from the [PyTorch Installation Page](https://pytorch.org/get-started/locally/).

Create a Python virtual environment using e.g. Conda:

```shell
conda create -n SimPER python=3.10 && conda activate SimPER
```

```shell
python -m pip install flash-attn --no-build-isolation
```

## Training Scripts

We provide four training config files for the four training setups reported in our paper. The training config is set for 4xA100 GPUs. You may need to adjust `num_processes` and `per_device_train_batch_size` based on your computation environment. 

* Mistral-Base:
```shell
bash Llama-8B-Base.sh
```

* Llama3-Base:
```shell
bash Mistral-7B-Base.sh
```


## Benchmarks

* [AlpacaEval repo](https://github.com/tatsu-lab/alpaca_eval) for evaluation.

* [Open LLM Leadboard v1](https://huggingface.co/spaces/open-llm-leaderboard-old/open_llm_leaderboard).

* [Open LLM Leadboard v2](https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard)  for evaluation.




