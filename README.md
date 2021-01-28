[Original jupyter notebook](/banking_dataset_gen(old).ipynb) that leverages a public [retail bank datset from the Czech Repulic](https://data.world/lpetrocelli/czech-financial-dataset-real-anonymized-transactions) and some of the work done by @namebrandon on [Sparkov Data Generation here](https://github.com/namebrandon/Sparkov_Data_Generation) to create a dataset for demo use showing Account + Credit Card transactons and payments. **Note that the code is stale and should just be used as a point of reference for logic

[New jupyter notebook](/cust_trans_gen.ipynb) that can be run to generate additional customers with different credit cards and transactions associated with the card. This notebook should be used by googlers with a service account that has write access to the retail_banking storage bucket and the finserv_staging BQ dataset in the Looker demo project. New customers / cards are added as a table to the staging schema in BQ and the transactions are written to CSV files delimited by a pipe in google cloud storage. Requirements for running the notebook can be found [here](/requirements.txt). Existing customers can be used from the [customers.csv file](/customers.csv).
