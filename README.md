I. Package Introduction:

    |-- State_Space: this package is used to generate daily state space and portfolio IR rank.
    |   |-- feat_selection.py:
    |   |-- Generate_IR_rank_week.py:
    |   |-- IR_month.py:
    |   |-- Update_IR_rank.py:
    |
    |-- data: this folder contains required data.
    |   |-- industry.csv :
    |   |-- industry_quote.xlsx :
    |   |-- nav.csv :
    |   |-- quote.csv :
    |   |-- records.csv :
    |   |-- IR_rank_week.csv :
    |
    |-- task1: stock trading.
    |   |-- Similarity_Search :
    |   |-- Supervised_Learning : in this folder, we realized a Supervised Learning method (Neural Network) to allocate stock weights.
    |
    |-- task2: portfolio management.
    |   |-- DDPGmodel: use DDPG model.
    |   |-- DQNmodel: use DQN model.
    |   |-- QLearningModel: use Q-learning model.
    |   |-- QLearningModel_beta: use Q-learning model and slide (train and test) window.
    |
    |-- base.py: some basic method used by all packages.
    |
    |-- run_model.py: main function of running a model.


II. How to run the model?

    1. Make sure to use Python 3.0+.
    2. Make sure to install all required third-part packages: [numpy, Keras, tensorflow, TA-lib, pandas, etc].
    3. Replace data files in ./data folder, the file name MUST BE same as above introduction.
    4. Update 'project_path' and start_date in ./run_model.py file.
          project_path='/Users/Youran/Projects/PortfolioManagement'
          start_date='2017-01-06' : that means our model will use data before 2017-01-05 to train a model, and make prediction based on 2017-01-06.
    5. [OPTIONAL] You can change 'train_window' size in ./run_model.py file.
          train_window = 10
    6. python ./run.py

III. BUG?

    Of course...
    If some strange error appear, calm down please, re-run it or contact me thx! email: cheeryouran@yeah.net
    Have a good day!
