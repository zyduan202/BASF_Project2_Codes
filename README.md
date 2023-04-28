# Project 2: Catalyst Design with Decision Trees and Shapley Additive Explanations

Zhaoyan Duan, Haotong Xie

## INTRODUCTION

Recently, machine learning (ML) has emerged as a promising tool for catalyst discovery and optimization. In particular, the paper "Identifying Descriptors for Promoted Rhodium-Based Catalysts for Higher Alcohol Synthesis via Machine Learning" by Suvarna et al. has demonstrated the potential of ML models for identifying key catalytic descriptors for higher alcohol synthesis process.

In this project, we aim to replicate the results presented in the paper, conduct a robustness check of the models, and apply alternative methods to compare and validate the findings. In addition, we observed that the controllable reaction conditions had a greater impact on the higher alcohol synthesis process than the catalytic descriptors of interest, and as such, we aim to investigate methods for reducing their influence and emphasizing the importance of the descriptors.

## OBJECTIVES

The project aims to achieve the following objectives:

• Replicate the results reported in the paper "Identifying Descriptors for Promoted Rhodium-Based Catalysts for Higher Alcohol Synthesis via Machine Learning".

• Perform a robustness check of the descriptive statistics and machine learning model analysis presented in the paper.

• Employ alternative methods to analyze the data and compare our findings with those reported in the paper.

• Explore ways to mitigate the influence of reaction conditions on the model's predictions and emphasize the importance of catalyst descriptors as input features.

By fulfilling these objectives, we intend to enhance our comprehension of the catalyst descriptors for higher alcohol synthesis and identify potential opportunities for advancement or further investigation.

## METHODOLOGY

Given the absence of a robustness check in the paper, we propose constructing confidence intervals and using Bootstrap resampling to validate the results. These methods will provide additional insight into the stability and reliability of the machine learning model. As alternative methods, we plan to implement a regression model with regularization and a deep learning model using a multi-layer perceptron (MLP) architecture to analyze the dataset used in the paper and identify the most significant input features. The use of regression models will provide a different perspective to the analysis. Furthermore, the small size of our dataset increases the risk of overfitting in machine learning models, while regularization techniques can mitigate this problem. Finally, MLPs have shown to be powerful tools for generalization tasks, which can provide us with a robust framework for prediction and classification.

## DATA

The data used in both the paper and our project is an open-source dataset on Rh-catalyzed higher alcohol synthesis (HAS) obtained from Pacific Northwest National Laboratory (PNNL). For our project, we have selected 19 catalytic descriptors as well as reaction conditions weather and gas-hourly space velocity as input features, resulting in a total of 225 datapoints.

## EVALUATION METRICS

In order to ensure comparability between the outputs obtained from alternative methods and the original results, we adopted the same evaluation metrics as those used in the paper, namely R2 (coefficient of determination) and RMSE (root-mean-square error).

## TIMELINE

Our project timeline is divided into three phases:

1. Replication and Validation Phase (March 2023 - May 2023)

   - Replicate the code and results presented in the paper

   - Conduct a robustness check to validate the results

   - Explore alternative methods to compare the findings

2. Feature Selection and Modeling Phase (May 2023 - July 2023)

   - Find solutions to suppress the influence of reaction conditions on catalytic performance

3. Refinement and Documentation Phase (July 2023 - September 2023)

   - Refine the models developed in the project

   - Obtain final results

   - Prepare a comprehensive term paper documenting the methodology, findings, and conclusions 

By following this timeline, we aim to successfully replicate the results presented in the paper and contribute new insights to the field of catalysis research. 

## CONCLUSION

In conclusion, this project aims to replicate the results presented in the paper "Identifying Descriptors for Promoted Rhodium-Based Catalysts for Higher Alcohol Synthesis via Machine Learning" and conduct a robustness check to validate the original findings. Through the exploration of alternative methods, we also hope to identify areas for improvement and contribute new insights to the field of catalysis research. By focusing on feature selection and modeling techniques, we aim to develop new models that highlight the effects of catalytic descriptors while suppressing the influence of reaction conditions. By following the proposed timeline and methodology, we anticipate a successful outcome and the potential to make a meaningful impact in the field of catalysis research.

## REFERENCES

Bishop, C. M. (2006). Pattern recognition and machine learning. Springer. 

Fahrmeir, L., Kneib, T., Lang, S., & Marx, B. (2013). Regression: Models,Methods and Applications. Springer Science & Business Media. 

Goodfellow, I., Bengio, Y., & Courville, A. (2016). Deep Learning. MIT Press. 

Richert, W. (2013). Building Machine Learning Systems with Python. Packt Publishing Ltd.

Stevens, E., Antiga, L., & Viehmann, T. (2020). Deep Learning with PyTorch. Simon and Schuster.

Suvarna, M., Preikschas, P., & Pérez-Ramírez, J. (2022). Identifying Descriptors for Promoted Rhodium-Based Catalysts for Higher Alcohol Synthesis via Machine Learning. ACS Catalysis, 12(24), 15373–15385. https://doi.org/10.1021/acscatal.2c04349 

Zhang, A., Lipton, Z. C., Li, M., & Smola, A. J. (2021, June 21). Dive into Deep Learning. ArXiv.Org. https://arxiv.org/abs/2106.11342v4 

Ziegel, E. R. (2003). The Elements of Statistical Learning. Technometrics, 45(3), 267–268. https://doi.org/10.1198/tech.2003.s770
