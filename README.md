# NBA Shot Predictor

### Overview

This project is an end-to-end Databricks data engineering and machine learning pipeline that predicts the probability of an NBA shot being made using shot-level context data and following a lakehouse-style bronze, silver, and gold architecture.



### Project Goal
The goal is to estimate whether an NBA shot will be made or missed based on features such as:
- Shot distance
- Closest defender distance
- Shot clock
- Game clock
- Period
- Touch time
- Dribbles
- Shot type
- Home/Away


### Dataset
This project uses a public NBA shot log dataset on 128,069 shots taken during the 2014-2015 season containing fields such as:
- GAME_ID
- MATCHUP
- LOCATION
- PERIOD
- GAME_CLOCK
- SHOT_CLOCK
- DRIBBLES
- TOUCH_TIME
- SHOT_DIST
- PTS_TYPE
- SHOT_RESULT
- CLOSEST_DEFENDER
- CLOSE_DEF_DIST
- FGM
- player_name
- player_id

### Tools Used
- Databricks
- Python
- PySpark
- Spark SQL
- Spark MLlib
- Delta tables


### Features Used
- is_close_shot
- is_mid_range_shot
- is_three_point_shot
- is_deep_shot
- is_very_tight_defense
- is_tight_defense
- is_open_defense
- is_wide_open_defense
- is_last_5_min_game
- is_last_2_min_period
- is_end_of_period
- shot_clock_adjusted
- is_shot_clock_missing
- is_very_late_clock
- is_late_clock


### Models Used
- Logistic Regression
- Random Forest Classifier