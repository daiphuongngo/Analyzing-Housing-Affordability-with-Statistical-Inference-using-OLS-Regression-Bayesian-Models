# Analyzing-Housing-Affordability-with-Statistical-Inference-using-OLS-Regression-Bayesian-Models

![Harvard_University_logo svg](https://github.com/user-attachments/assets/c4916307-eb16-43a2-85f8-6ab6f783ceea)

![Harvard-Extension-School](https://github.com/user-attachments/assets/fbc74fc8-266c-4262-813c-f7f8bbd05a96)

## **Master of Liberal Arts, Data Science**

## **CSCI E-83 Fundamentals of Data Science in Python**

## Professor's name: **Stephen Elston**

## Author's name: **Dai Phuong Ngo (Liam)**

# **Analyzing Housing Affordability: Exploring Key Influential Features by Regression and Statistical Modeling**

# **Introduction and Background**

The housing market has long been a crucial area of interests for businesses, individuals and especially policy makers. In the mortgage banking industry where I am working for at the moment, understanding factors impacting on housing affordability is critical for tailoring financial products, advising clients and managing risks from different perspectives. In Canada particularly, housing affordability has become increasingly challenging due to rising sales prices, limited inventory because of slow construction versus high demand, and economic uncertainty. This triggered the requirement for mortgage providers and underwriters, real estate brokers, consumers to evaluate the most influential factors driving housing affordability.

The issues might face complexity due to the wide range of direct features impacting on sales price, such as living space, condition, property type or less obvious features, such as, year remodeled or basement size. An unwanted fact is that the distribution of sales price is often skewed with extreme outlers complicating further analysis. Traditional evalutions might not succeed in understanding all of these variations, therefore, empowering advanced statistical techniques is important to understand and diagnose affordability better.

# **Project Goal**

This project aims to analyze the key housing features that affect sales prices and housing affordability to provide actionable insights. Inferences retrieved from the data can help to identify features having greatest impact on affordability and generate further insights for homebuyers, who have to make informed decision on which housing option is compatible with their affordability, real estate brokers, who have to customize advice and recommendations to individual needs, and mortgage providers or banks, like my current company, who have to set up financing solutions based on metrics of housing affordability. Therefore, the final goal of this project is to develop statistical solutions with sampling techniques, OLS regression models and Bayesian analysis to assess contributions from the most influential housing features to housing affordability. This emphasis will be on inference, rather than prediction, and will address upcoming challenges expressed by skew distributions in prices and their outliers to make sure conclusions are drawn in a statistically reliable, practical and relevant way.


# **What This Project Is Not About**

It is import to clarify that this project is not about price prediction or prediction's optimization. Instead, it concentrates on statistical inference, which determines the impact of different features on affordability and provides a statistical framework to interpret their impacts to indentify the most crucial influencers. Machine Learning algorithms such as tree-nased models or neural networks are not applicable in this project as it focus on capturing relationships among features. Also, this project does not set certain affordability thresholds manually and affordability's classification.


# **Data**

A challenge arises with the data availability for the Canadian context that I am unable to find a good enough or ready-to-consume data with domain in Canadian housing affordability. I tried to look through websites of Government of Canada or Canada Statistics but their data are scattered, not yet combined, time series type and require significant amount of time to find enough data aspects for manipulationa and combination, regarless of their individual dataset's completeness across features. Therefore, I decided to focus on statiscal modelling techniques analyzing housing affordability with usage of this data from the American housing context of Ames city.

The data comes directly from Kaggle with two sets: training and testing. I will use the training for data exploration, preparation, assessment and model development before applying the best model on the testing set. The data has 79 explanatory variables which are manageable and describe aspects of residential properties in Ames, Iowa. This data provides an excellent source to study housing trends and affordability with a good amount of meaningful features and data records describing different aspects of housing. The modelling will take all features as influencers to be analyzed, visualized, sampled and modelled to assess the final set of best features on different samples of the US house prices and affordability in Ames. Later, the training data can be split into 2 samples: training and testing for further model evaluation.

https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques


# **Project Proposal**

The project I would like to work on for this course is the continuation on the House Prices - Advaced Regression Techniques from Kaggle. Serveral years ago I started exploring my basic skills in EDA, Machine Learning and Deep Learning and visualization with this dataset. However, as I'd like to move upward to become Data Scientist in the near future, applying what have been taught in the Master's classes in terms of diagnostics, inferences and sampling techniques for this project to analyze factors contributing to housing affordability. As I have joined a new company recently in the banking industry of mortgage, analyzing data related to housing is crucial, especially in terms of Risk and Mortgage Product as well as Marketing. However, finding a good enough data like this Kaggle's one for the Canadian market is a challenge as I have been finding one from Government of Canada or private sources but the governmental data seems to be very condensed, scattered and hard to merge or union. Canadian housing affordability has experiencing many challenges due to different factors, such as immigration, shortage of jobs, unemployment rate, consumer behavior, interest rate, etc... so it might be similar to or different from the US. Finding or concatenating more data with more features is very time-consuming and a lot of effort. Therefore, I circle back to this data from Kaggle as a reliable dataset with adequate features as a starting point to dive deeper into more descriptive, diagnostic, sampling, inferences, regression and Bayesian model applications learned from this course.

# **Final Summary**

My project involves analyzing housing affordability using Bayesian hierarchical and unpooled models. Key features such as neighborhood attributes, numerical housing characteristics, such as bedrooms, lot sizes, and categorical factors, such as building type, house style, were included.

**Data Preparation**:

I processed and standardized numerical features as well as converted categorical variables into one-hot or binary numerical formats. I also removed missing values to ensure data integrity.

**OLS Regression**:

Built an OLS model as a baseline for analyzing housing price determinants. Key findings from OLS are that GarageCars and TotalBath were significant positive predictors of housing prices. Neighborhoods and categorical features such as BldgType and HouseStyle had a meaningful impact on affordability. Limitations identified with OLS are that it assumes homoscedasticity and independent errors, which may not capture hierarchical dependencies, such as neighborhoods.

**Bayesian Modeling**:

I developed Hierarchical Models with group-level effects (neighborhoods) using Laplace priors for interpretability in intercepts and coefficients. I also built an Unpooled Model for fully independent parameter estimation as well as a Pooled Model for independent parameter estimation regardless of neighborhood, and compared results using trace plots, posterior summaries and posterior predictive checks.

**Correlation Analysis**:

I examined relationships between key numerical features using Spearman and Pearson correlation matrices to identify significant predictors and features with multicollinearity for complexity reduction.

**Insights**:

Hierarchical models revealed varying neighborhood-level affordability trends. Unpooled models highlighted independent effects of specific features, like GarageCars and TotalBath, on housing affordability. Categorical variables such as BldgType and HouseStyle demonstrated significant predictive power.

**Statistical Inference**:

Posterior distributions provided credible intervals for coefficients, aiding decision-making. Insights support identifying key drivers of affordability and potential areas for policy intervention.

**Impact**:

My analysis offers a robust framework for housing market insights, combining OLS regression for interpretability and Bayesian techniques for flexibility and precision. It supports policymakers and stakeholders in understanding affordability drivers at both micro and macro levels. When new data and information are provided to embed with the past data, the posterior insights from my current Bayesian models can be used as prior information or beliefs for the new Bayesian models fitted with a combination of old and new data to update posterior insights.

# **Further Improvement**

Further Bayesian analysis applied time series data to analyze switchpoint of Economic crisis from Dec 2007 - June 2009 impacting the target and housing affordability and tracking how an event or policy can affect the trend based on causal inference. This modelling would require more sophisticated techniques handling factors contributing to priors, switchpoint and posteriors. Time series data often exhibit structural breaks or regime changes, such as sudden changes in trends so standard Bayesian models may fail to adapt to these changes. Also, choosing appropriate priors is critical but non-trivial, especially in high-dimensional time series datasets because poorly chosen priors can lead to biased or unstable posterior estimates. Therefore, in my current project, I have not extended to conduct more research on this analysis.

# **References**

Diagnosing Biased Inference with Divergences

PyMC Team. "Diagnosing Biased Inference with Divergences." PyMC Examples: Diagnostics and Criticism. Link at: https://www.pymc.io/projects/examples/en/latest/diagnostics_and_criticism/Diagnosing_biased_Inference_with_Divergences.html

Hierarchical Modeling with Variational Inference

PyMC Team. "Hierarchical GLM with ADVI and Minibatch." PyMC Examples: Variational Inference. Link at: https://www.pymc.io/projects/examples/en/latest/variational_inference/GLM-hierarchical-advi-minibatch.html

Rugby Analytics with Bayesian Hierarchical Models

PyMC Team. "Bayesian Hierarchical Models in Rugby Analytics." PyMC Examples: Case Studies. Link at: https://www.pymc.io/projects/examples/en/latest/case_studies/rugby_analytics.html

Hierarchical Binomial Model with PyMC

PyMC Team. "GLM: Hierarchical Binomial Model." PyMC Examples: Generalized Linear Models. Link at: https://www.pymc.io/projects/examples/en/latest/generalized_linear_models/GLM-hierarchical-binomial-model.html

Hierarchical Partial Pooling

PyMC Team. "Hierarchical Partial Pooling: A Case Study." PyMC Examples: Case Studies. Link at: https://www.pymc.io/projects/examples/en/latest/case_studies/hierarchical_partial_pooling.html

Bambi: A High-Level Bayesian Modeling Interface

Bambi Developers. Bambi: Bayesian Models Made Easy. Link at: https://bambinos.github.io/bambi/

