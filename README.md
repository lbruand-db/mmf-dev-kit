# Many-Model Forecasting (MMF) Dev Kit

A focused development kit for the **Many-Model Forecasting** skill, enabling AI coding assistants to build time series forecasting pipelines on Databricks.

## What's Included

| Component | Description |
|-----------|-------------|
| [`databricks-skills/many-model-forecasting/`](databricks-skills/many-model-forecasting/) | The MMF skill — patterns and best practices for forecasting on Databricks |
| [`.test/`](.test/) | Test infrastructure for evaluating the skill |

## The MMF Skill

The Many-Model Forecasting skill teaches AI assistants how to:

- Build forecasting pipelines using **MMF Solution Accelerator** (`mmf_sa`)
- Use statistical models (**StatsForecast**) and neural models (**NeuralForecast**)
- Run **Chronos** foundation models for zero-shot forecasting
- Orchestrate many-model training across Databricks clusters

## Running Tests

From the `.test/` directory:

```bash
# Unit tests
uv run --extra dev python -m pytest tests/test_scorers.py -v

# Skill evaluation
uv run --extra dev python scripts/run_eval.py many-model-forecasting
```

## License

(c) 2026 Databricks, Inc. All rights reserved.

The source in this project is provided subject to the [Databricks License](https://databricks.com/db-license-source). See [LICENSE.md](LICENSE.md) for details.
