# Computational Statistics Analysis on MNIST Digit Classification Result - 

### How Could Object Shape & Size Relate to Prediction Biases?

###### * Umich STATS 406 *(Computational Method in Statistics)* Fall 23 Final Project

###### - Generated and organized by Ziming Zhou

## Project Summary

This project utilizes advanced computational statistical methods to meticulously investigate biases stemming from object size and shape in image classification, with a focus on the MNIST dataset. The methodology incorporates a robust approach to ensure the reliability and depth of the analysis. Quantile-Quantile plots, Violin plots, and bootstrapped skewness diagnostics are employed for the rigorous examination of feature normality, allowing for a detailed scrutiny of the distributional characteristics of extracted features. Stratified sampling from long-tailed distributions provides a solid framework for assessing biases in prediction probabilities. The permutation test for asymmetricity detection effectively stratifies the probability range, revealing nuanced patterns of bias in low-confidence and high-confidence samples. Simulation results, including the effective use of permutation tests to examine decay rates and bootstrapping for analyzing noisy normal distributions, validate the chosen methodologies, underscoring their applicability across diverse scenarios. These computational statistical methods not only enhance the credibility of the analysis but also contribute to the project's overarching goal of unraveling biases in image classification with a nuanced and data-driven approach.

## File Directory

| File Name                           | Content                                                      |
| ----------------------------------- | ------------------------------------------------------------ |
| 0-0.3-500.csv                       | Original Low-prob Data: Prob $\in$ [0-0.3] 500 Samples       |
| 0.3-0.7-158.csv                     | Original Mid-prob Data: Prob $\in$ [0.3-0.7] 158 Samples     |
| 0.7-1-500.csv                       | Original High-prob Data: Prob $\in$ [0.7-1] 500 Samples      |
| 3-region-bootstrap.csv              | Raw result of bootstrapping mean & variance on three regions, generated from "res-code.Rmd" |
| sampled_low_pred_conf1.csv          | Sampled Low-prob Data: Prob $\in$ [0-0.3] 150 Samples, generated from "res-code.Rmd" |
| sampled_high_pred_conf2.csv         | Sampled High-prob Data: Prob $\in$ [0.7-1] 150 Samples, generated from "res-code.Rmd" |
| prediction.csv                      | The NN prediction result of 20,000 validation set sample, 20,000 rows * 10 column, each column represents the corresponding prediction probability from digit [0] to [9] |
| ./Digit_Avg_Test/*_data.csv         | Image-based Feature Extraction Result of every corresponding digits used for digit-wise distribution analysis |
| ./Digit_Avg_Test/**Digit-Test.Rmd** | Code for digit-wise distribution generation and analysis     |
| **res-code.Rmd**                    | Code for reproducing results from the Result & Analysis Section |
| **sim-code.Rmd**                    | Code for reproducing results from the Simulation Section     |

## Final Project Paper

You can view our final project paper [here](./Final_Report/Report.pdf)
