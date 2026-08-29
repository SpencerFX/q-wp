# q-wp

A collection of companion code for **kdb+/q technical whitepapers and blog posts**
published by KX (formerly Kx Systems) at [code.kx.com/q/wp](https://code.kx.com/q/wp/)
and [kx.com/blog](https://kx.com/blog/).

Nothing here is original: each subdirectory is the code that ships alongside a KX
whitepaper, gathered in one place for convenience. Refer to the linked papers for
the full explanation of what the code does and why.

## Contents

All papers live under [`kx/`](kx/).

| Directory | Whitepaper / post | Topic |
|-----------|-------------------|-------|
| [`kx/embedpy-lasso`](kx/embedpy-lasso) | [Machine Learning: using embedPy to apply LASSO regression](http://code.kx.com/q/wp/embedpy-lasso) | embedPy, LASSO regression on housing prices (Jupyter notebook) |
| [`kx/market-fragmentation`](kx/market-fragmentation) | [Market Fragmentation: a kdb+ framework for multiple liquidity sources](https://code.kx.com/v2/wp/market-fragmentation/) (Jan 2013) | Consolidating multiple liquidity sources |
| [`kx/massIngestionDataloader`](kx/massIngestionDataloader) | [Mass ingestion through data loaders](https://code.kx.com/q/wp/data-loaders/) | Orchestrator/worker CSV ingestion into an HDB |
| [`kx/oauth2`](kx/oauth2) | [OAuth2 authorization using kdb+](https://kx.com/blog/oauth2-authorization-using-kdb/) | OAuth2 client flow in q |
| [`kx/q-signals`](kx/q-signals) | [Signal processing and q](http://code.kx.com/q/wp/signal-processing) | Complex numbers, Radix-2 FFT, timeseries anomaly detection |
| [`kx/trend-indicators`](kx/trend-indicators) | [Implementing trend indicators in kdb+](https://code.kx.com/q/wp/trend-indicators/) | Trade analytics: indicators and oscillators, crypto feed |
| [`kx/websocket`](kx/websocket) | [kdb+ and WebSockets](https://code.kx.com/q/wp/websockets/) | Browser <-> q via `.z.ws`, pub/sub, live tables |
| [`kx/wp-knn`](kx/wp-knn) | [Machine Learning in kdb+: k-Nearest Neighbor classification](http://code.kx.com/q/wp/machine_learning_in_kdb.pdf) | k-NN classifier, digit recognition, benchmarking |

Each subdirectory has its own `README.md` with run instructions specific to that paper.

## Requirements

- **kdb+ / q** (a recent 3.x or 4.x build). Get it from [kx.com/kdb-personal-edition-download](https://kx.com/kdb-personal-edition-download/).
- Some papers need extras:
  - `embedpy-lasso`, `q-signals` — [embedPy](https://code.kx.com/q/ml/embedpy/) and Jupyter ([JupyterQ](https://code.kx.com/q/ml/jupyterq/)) for the `.ipynb` notebooks.
  - `trend-indicators` — Python 3 (`crypto.py` pulls a cryptocurrency feed into a tickerplant).
  - `websocket` — any modern web browser for the HTML demos.

## License

Apache License 2.0 — see [LICENSE](LICENSE). Individual whitepaper directories may
carry their own upstream license (e.g. [`kx/wp-knn/LICENSE`](kx/wp-knn/LICENSE)).
