# schnell.AI Examples
## classification-iris

### Summary
This example provides a simple classification-project. This project will classify iris-flowers by their petal and sepal length an width.

### Artifacts
| Name                 | Type                 | Importer | Exporter | Description                                                    |
|----------------------|----------------------|----------|----------|----------------------------------------------------------------|
| data_training        | Training-Dataset     | CSV      |          | CSV file with training-data                                    |
| data_evaluate        | Evaluation-Dataset   | CSV      |          | CSV with data to evaluate                                      |
| data_results         | Result-Dataset       |          | CSV      | CSV with evaluation data including result class and confidence |
| model_classification | Classification-Model |          |          | Classification-Model                                           |

### Components
| Name            | Type                  Description                                                                  |
|-----------------|----------------------------------------------------------------------------------------------------|
| action_evaluate | Classification-Evaluator|Evaluates data from 'data_evaluate' with the model 'model_classification' |
| action_train    | Classification-Trainer|Trains model 'model_classification' with data from 'data_training'          |
