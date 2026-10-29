# aeolus
Model -1: AEP calculation: Based on physics and Estimation correction
AEP correction with relative real life data.
USwind data

Model -2: Turbine placement
turbine placement model to optimize path, direction of hub, hub height based on the database of turbines available for best output and location

0.1v: will not do: wake prediction, CFD


Success Criteria:

A. Working ML model
Pass criteria
- Creation of windrose, from past data, and explain the reason behind the windrose variation and affect on AEP variation over the year.
- Direct numerical Estimation of AEP over a year around segment.
- The saved model can be loaded again and used to make a prediction.
- Invalid or missing inputs produce a clear error rather than a misleading result.



B. Baseline comparison
Pass criteria
- A simple persistence baseline is implemented: predict that year, wind AEP calculation on fixed height.
- The ML model and baseline are evaluated on exactly the same test timestamps.
- MAE and RMSE are reported for both.
- You can clearly state whether the ML model improves on the baseline.



C. Honest evaluation
Pass criteria
- Training data comes before validation data, which comes before the final test period.
- Information from the future is not accidentally used to predict the past or future.
- Final test results are reported even if they are disappointing.
- Limitations of the dataset and model are documented.



D. Usable interface
Pass criteria
- A user can enter or select the required inputs and run a prediction.
- The interface displays the prediction, units, timestamp, and baseline comparison.
- Errors are understandable to a nontechnical user.
- The interface clearly states that a wind-speed prediction is not measured turbine electricity generation.



E. Reproducible results
Pass criteria
- The dataset source, processing steps, and model settings are recorded.
- The code and environment instructions are documented.
- The saved model can be reloaded and tested.
- Re-running the evaluation using the same data and settings reproduces the reported metrics within a defined tolerance.