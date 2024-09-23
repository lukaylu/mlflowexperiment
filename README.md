## ML Flow Experiments

import dagshub
dagshub.init(repo_owner='lukaylu', repo_name='mlflowexperiment', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)