**Project description:** 

Many companies rely on VMWare NUMA's advanced server platforms to run their business applications. 
Default settings can lead to misconfigurations of the server settings and thus inflated server costs. But most companies don't know in advance which misconfigurations will reduce costs enough to justify the time and costs of a fix.


### 1. Hypothesis

Case-specific predictions of performance increases could help operations teams to estimate the impact of investments in reconfiguration in order to better prioritize maintenance spending. 

Market research indicates that there is no known commercial solution, so any predictions more reliable than guesswork could be useful. 


### 2. Assumptions 

- Sufficient data to capture the shifting relationships between configurations settings, usage trends, and different system architectures/versions. Some may be easier to model than others.
- Key drivers are represented in the available data sets.


### 3. Statistical tools and techniques

Data processing [latest version of the python code here] (/anonymized_data_processing.html)
- Aggregation of data from reporting and logging
- Merge data from different sources (logging from hosts vs. virtual machines)

Modelling notebooks [latest version of the python notebook here] (/mpno_simple_vm-host_models-vm-environment4-v2.html)
- Feature engineering to generate new variables, including synthetic usage statistics used in projections
- Experimented with several regression models: Multiple linear regression, decision tree, random forest, xgboost regressor


### 4. Outlook

If the pilot project proves successful, our partner will propose further development to additional clients.

The best models in the first phase of the project had explained variance scores in the .80-.85 range. The next steps include further testing of these models against a variety of use cases, as well as additional model optimimization.

