There are three methods adaptive scaling employs to make it work.

Machine Learning (ML) Models
–
ML models are used to predict application transactions per second. There are currently three models in production:
1. XGBoost (adaptive scaling)
2. ARIMA (predictive scaling)
3. Fourier Transforms (seasonality prediction)


Calculated Scaling
–
HTTPS requests per second are calculated, and the application is scaled for real-time TPS (transactions per second) requirements.


Protective Metrics
–
When an anomaly is detected in select metrics (cpu_throttling, restarts, and p50latencyspike), the application is scaled dynamically to mitigate the impact.
