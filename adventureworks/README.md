cd dbt-dimensional-modelling/
python3.8 -m venv dbt_venv
source dbt_venv/bin/activate
pip install -r requirements.txt
cd adventureworks/
Open profiles.yml file and edit your Snowflake Credentials
dbt deps
dbt seed --target snowflake
