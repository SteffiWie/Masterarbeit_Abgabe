# Masterarbeit_Abgabe

## Introduction

Algorithm selection in time series classification, which involves mapping ordered sequences of data points to discrete target variables, is critical to ensuring successful classification on real-world time series data. This problem is crucial because algorithms exhibit varying performance on different data sets. Existing research in automated machine learning and its subfields, such as meta-learning, hyperparameter optimization, and neural architecture search, contribute significantly to automating algorithm selection. These approaches primarily focus on prediction performance but neglect the influence of uncertainties in the data and in the prediction process on the selection. 

This thesis investigates regression models that can quantify these uncertainties and attribute them to their sources, and evaluates their suitability for more interpretable performance prediction in the context of time series classification algorithms. We design toy problems that allow us to evaluate whether the identified models can quantify uncertainty due to performance variance or data limitations and how the representation of the time series data set affects the uncertainty in the performance prediction. Our findings suggest that the identified models are promising in quantifying uncertainties and attributing them to their source. A sufficient database is crucial for accurate performance prediction. In particular, the representation of time series datasets plays a key role in correctly identifying sources of uncertainty. By incorporating uncertainty estimation into performance prediction, our work enhances interpretable algorithm selection, while also providing a foundation for future research.

## Information

This code is part of my master thesis.

Three regression models 

- random forest (RF) trained on aggregated data
- virtual stochastic Langevin Boosting (vSGLB)
- gaussian process regression (GPR)
  
are identified for their suitability for algorithm selection of an time series classification algorithm that can quantify uncertainties in their performance prediction.

## Quickstart - How to run the code

The code was developed and tested on Python 3.11.11.

1. Clone the repository
   ```bash
   https://github.com/SteffiWie/Masterarbeit_Abgabe.git  
    ```
2. Install dependencies
```bash
pip install -r requirements.txt
```
3. Run the different toy problems.
   ```bash
    /toy_1.ipynb
    ```
    ```bash
    /toy_2.ipynb
    ```
    ```bash
    /toy_3.ipynb
    ```

## Toy Problem 1

This toy problem qualitatively assesses how well the selected regression models quantify aleatoric and epistemic uncertainties in the presented toy problem and thus address the question of how well the uncertainties can be attributed to their sources.

## Toy Problem 2

This toy problem qualitatively assesses the effects of an increase in the number of training points, in particular, on the quantification of epistemic uncertainty. The effects can be interactively visualized.

## Toy Problem 3

This toy problem qualitatively assesses the effects of introducing one or more additional meta-features to distinguish instances on the quantified uncertainties.


