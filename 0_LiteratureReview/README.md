# Literature Review

Approaches or solutions that have been tried before on similar projects.

**Summary of Each Work**:

- **Source 1**: [Improving Global Stock Market Prediction with XGBoost and LightGBM]

  - Guennioui et al. (2023) https://refpress.org/wp-content/uploads/2024/02/Guennioui_REF.pdf
  - **Objective**: Evaluate XGBoost, LightGBM, and their hybrid in forecasting stock prices across multiple markets.
  - **Methods**: Trained both models (with unified hyperparameters) and a combined ensemble model, using standard features and global datasets.
  - **Outcomes**: Ensemble outperformed individual models across markets; LightGBM and XGBoost showed comparable performance, particularly in stable markets
  - **Relation to the Project**: Supports our finding that tree‑based ensemble methods perform similarly and robustly across varied stocks, just as we observed.

- **Source 2**: [Evaluating the Performance of Machine Learning Algorithms in Financial Market Forecasting: A Comprehensive Survey]

  - Ryll & Seidens (2019)  https://arxiv.org/abs/1906.07786
  - **Objective**: Review and compare over 150 studies applying ML to financial forecasting, evaluating models like ANN, SVM, Random Forest, XGBoost, and RNNs.
  - **Methods**: Meta-analysis using published performance metrics (RMSE, MAE) and rank comparisons across model types
  - **Outcomes**: ML models generally outperform traditional statistical approaches. RNNs often outperform feed-forward networks and SVMs, indicating value in capturing temporal dependencies
  - **Relation to the Project**: Helps justify using varied model architectures (trees, RNNs, feed‑forward) in our pipeline; aligns with our comparative approach

- **Source 3**: [N‑BEATS: Neural Basis Expansion Analysis for Interpretable Time Series Forecasting]

  - https://arxiv.org/pdf/1905.10437
  - **Objective**: Propose a new feed‑forward architecture tailored for univariate time series forecasting.
  - **Methods**: tack fully connected “blocks” with residual backcast and forecast outputs; trained and evaluated on benchmark datasets (M3, M4, tourism).
  - **Outcomes**:  Achieved state‑of‑the‑art results, outperforming both classical methods and recurrent models like RNNs/LSTMs
  - **Relation to the Project**: Baseline for our N‑BEATS implementation; supports why a feed‑forward architecture can be as effective (or more) than RNNs for return prediction.
