## Training Record

| **Index** | **WRMSEE in last 28 days** | **WRMSEE in leaderboard** | **description** |
|-----------|----------------------------|---------------------------|-----------------|
| submission_1 | 0.86077 | 0.88913 | HTS group by store_id, disaggregation by historical averages<br/> LSTM setting: 1024 neuron, MSE, adam, 100 epochs | 
| submission_2 | ? | 0.78902 | HTS group by store_id, disaggregation by historical averages (last year)<br/> LSTM setting: 1024 neuron, MSE, adam, 100 epochs <br/> embedding cat var: (weekday, event_name, event_type) -> (3,7,3) |
| submission_3 | 0.6675 | 0.77858 | HTS group by store_id, disaggregation by historical averages (last 180 days)<br/> LSTM setting: 1024 neuron, MSE, adam, 100 epochs <br/> embedding cat var: (weekday, event_name, event_type) -> (4,10,4) |
