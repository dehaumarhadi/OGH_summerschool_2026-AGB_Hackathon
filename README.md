### Aboveground biomass modeling via Earth Observation
#### Data are prepared by OpenGeoHub Summerschool 2026

##### 1. Data preparation
- Data cleaning
- Add variables: NDVI and ECHOSAT (multi-years)
- Used variables: 'angle_palsar_xxxx', 'b02_s2.cdse.quarterly_xxxx0401_xxxx0631', 'b04_s2.cdse.quarterly_xxxx0401_xxxx0631', 'b08_s2.cdse.quarterly_xxxx0401_xxxx0631', 'bioregion', 'forest_type', 'HH_dB_palsar_xxxx', 'HV_dB_palsar_xxxx', 'obs_s2.cdse.quarterly_xxxx0401_xxxx0631', 'qa_palsar_xxxx', 'vh.sentinel1_xxxx07', 'vv.sentinel1_xxxx07', 'ndvi', 'canopy_height_2018','canopy_height_2019','canopy_height_2020','canopy_height_2021'

##### 2. Training strategy
- Model: LGBM regressor (n_estimators = 5000; num_leaves = 40; learning_rate = 0.1)
- Data split for train and test
- Data downsampling to make them balanced
- Accuracy evaluation

##### 3. Predict on test data for competition
