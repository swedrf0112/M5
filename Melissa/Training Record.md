## Submission Record

| **Index** | **WRMSEE in last 28 days** | **WRMSEE in leaderboard** | **description** |
|-----------|----------------------------|---------------------------|-----------------|
| submission_1 | 0.86077 | 0.88913 | HTS group by store_id, disaggregation by historical averages<br/> LSTM setting: 1024 neuron, MSE, adam, 100 epochs | 
||
| submission_2 | ? | 0.78902 | HTS group by store_id, disaggregation by historical averages (last year)<br/> LSTM setting: 1024 neuron, MSE, adam, 100 epochs <br/> embedding cat var: (weekday, event_name, event_type) -> (3,7,3) |
||
| submission_3 | 0.6675 | 0.77858 | HTS group by store_id, disaggregation by historical averages (last 180 days)<br/> LSTM setting: 1024 neuron, MSE, adam, 100 epochs <br/> embedding cat var: (weekday, event_name, event_type) -> (4,10,4) |
||
| submission_4 | 0.64159 | 0.76320 | HTS group by store_id, disaggregation by historical averages (last 180 days)<br/> BiLSTM setting: 1024 neuron, MSE, adam, 100 epochs <br/> embedding cat var: (weekday, event_name, event_type) -> (4,10,4) |
||
| submission_0410 | 0.52110 | 0.60778 | LSTM dropping first 1000 days data with features:<br/> * price_pct_change <br/> * price_discount <br/> * price_roll_std_7 <br/>  * demand_lag_28 <br/> * demand_lag_35 <br/> * demand_lag_42 <br/> * demand_lag_49 <br/> * roll_mean_7 <br/> * roll_mean_30 <br/> * roll_mean_60 <br/> * roll_mean_90 <br/> * roll_mean_180 <br/> * roll_std_7 <br/> * roll_std_30 <br/> * id var (OrdinalEncoding) <br/> * date var (Ordinal Encoding) <br/> LGBM parameter : <br/> * objective: 'poisson' <br/> * lr: 0.08 <br/> * lambda: 0.1 <br/> * num_leaves: 63 <br/> * bagging_fraction: 0.7 <br/> * bagging_freq: 1 <br/> * colsample_bytree: 0.7 <br/> * num_boost_roun<br/> * early_stopping_rounds: 400|
