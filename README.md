# Preparing Loans and Making Predictions

This repository contains the code used to process the kaggle loans dataset for training by DataRobot AutoML, and also the resulting predictions and explanations for a set of holdout loans

- Extract loans.csv from https://www.kaggle.com/wendykan/lending-club-loan-data/data
- Run code <b>Process Lending Raw Data</b> notebook to remove target leakers and add a loanID
- The notebook creates the file <b>training.csv</b>
- DataRobot automatically built 80 models from the training data to predict defaulted loans (yes or no)
- An <b>xgboost</b> model was recommended for deployment with threshold of 0.1493
- The deployed model was used to score loans in <b>scoring.csv</b>
- The resulting predictions and top 3 explanations are in <b>pred_reasons.csv</b>
