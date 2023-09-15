### Machine Learning

—— 

#### Supervised Approach:

- Feature Matrix : X
    - 2 dimensional array
    - Rows: observation objects
    - Columns: features
- Target: y


We have a feature matrix, and we want to predict y

Training function g <- model, takes in matrix X, and produces something close to y
 
Goal of ML train / come up with the function G that takes in the matrix, and produces something that is as close as the target as possible.

Supervised Machine Learning:
- Regression: many outcomes: infinite values possible
- Classification: We output a category
    - Multiclass:
        - many classes to choose from
    - Binary
        - two choices
            - eg: spam or not
- Ranking: Recommender Systems
    - Function that ranks items in an ecommerce website, and figures out what the most relevant for me to buy


#### CRISP-DM

cross industry standard process - for data mining

- Business Understanding
  - Do we need this?
  - how many people need this?
  - is it viable?
- Data Understanding
  - the case of a spam button
    - do we always track clicks
    - is the data being recorded
    - is the data reliable?
    - is the data large enough?
    - it may influence the goal
    - we may go back and see what we can do
- Data Preparation
  - Transform in such a way that can be put into an ML algo
  - feature engineering
    - extract features
  - clean the data
  - tabular format (matrix) = X
- Modeling
  - Try different modles
  - select best one
    - logistic regression
    - decision tree
    - NN
    - many others
    - we may need to add more features, fix data issues
- Evaluation
  - Go back to business understanding to see how the model is performing
  - retrospect whether the results required are attainable
- Deployment
  - Eval + Deploy usually go together
  - Online Evaluation
  - Deploy the model, evaluate it
  - canary deployment
  - focused on engineering
    - operationalize
    - monitoring
    - quality
    - maintainability
- ITERATEEEEE

#### Modeling

We can put away 20% of the data set to validate.
  - this is important because we need some ground truth to see how the model is performing
  - Multiple Comparisons
  - Probabilistic
  - Validation & Testing
    - take 20% to validate
    - Compare
    - One extra round of 20% to validate that the model we think its best, is the best.
    - 
What one more thing we need to keep in mind, is that once we select a model, we can reintegrate the validation 20%
into the training data, so that is not wasted.

We still keep the 20% test data so that we can still validate once the validation data is added to the training data.


Model Selection Process, one of the most important things in ML










