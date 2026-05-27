# clinical-trial-optimization

AI-based clinical trial design optimization platform for Phase II Type 2 Diabetes trials.

## Research Poster

View the project poster here:

[Research Poster](./docs/research-poster.pdf)

## Team

**Korean Minjok Leadership Academy, 29th Wavers**

### Development

- Minjoo Lee
- Haeun Jin

### Economic Research

- Gaeun Kim
- Sooin Lee

## Overview

**clinical-trial-optimization** is a web-based research prototype designed to explore how artificial intelligence can support more efficient clinical trial design.

The platform focuses on **Phase II clinical trials for Type 2 Diabetes** and simulates how different trial design choices may affect:

- Predicted trial success probability
- Estimated trial duration
- Estimated development cost
- Cost savings from AI-assisted optimization
- ROI efficiency under different revenue assumptions

This project aims to show how AI-assisted decision support can help researchers compare clinical trial design scenarios before implementation, reducing unnecessary cost and time while maintaining scientific reliability.

## Project Purpose

Clinical trials are expensive, time-consuming, and highly sensitive to early design decisions. Factors such as participant size, trial duration, control group type, blinding method, and primary endpoint can significantly affect the success, cost, and efficiency of a trial.

Traditionally, these design choices often depend on prior literature, expert judgment, and limited comparisons between possible trial structures. However, the number of possible design combinations is large, making it difficult to identify efficient trial designs manually.

This project investigates whether an AI model can support clinical trial design optimization by predicting trial success probability and comparing economic outcomes across alternative design scenarios.

## Key Features

### 1. AI Model Simulator

The AI Model Simulator allows users to adjust major clinical trial design variables and observe the predicted success probability in real time.

Input variables include:

- Number of participants
- Trial duration
- Control group type
- Blinding method
- Primary endpoint

The model uses only variables that are available during the trial design stage. This helps prevent data leakage and makes the system more relevant as a practical decision-support tool.

### 2. Economic Impact Simulator

The Economics section estimates the potential financial impact of AI-assisted clinical trial optimization.

It compares:

- Original trial duration
- AI-optimized trial duration
- Original estimated development cost
- AI-optimized estimated development cost
- Cost savings
- ROI efficiency

A simplified cost model is used to estimate trial cost based on trial duration and daily operating cost.

### 3. Visual Analysis

The platform includes visualizations that help users understand model performance and economic impact, such as:

- Trial duration distribution
- Trial cost distribution
- Cost comparison charts
- ROI-related indicators
- Trial dataset table

These visual elements are intended to make the research results easier to interpret and communicate.

## Research Background

The project is based on the idea that improving clinical trial design efficiency can create broader economic and social benefits.

For pharmaceutical companies, reducing clinical trial cost and duration may improve R&D efficiency and allow resources to be allocated to more candidate treatments.

For patients and society, more efficient clinical trials may contribute to earlier drug availability and potentially lower long-term healthcare costs, especially for chronic diseases such as Type 2 Diabetes.

## Methodology

The research process included the following steps:

1. Collecting and referencing public clinical trial information related to Type 2 Diabetes and Phase II trials
2. Building a structured dataset that reflects major clinical trial design variables
3. Training machine learning models to predict trial success probability
4. Comparing model performance and selecting a practical prediction model
5. Simulating alternative trial design combinations
6. Estimating cost and duration under traditional and AI-assisted scenarios
7. Building a web-based visualization platform to present the results interactively

## Model Summary

The project compares machine learning approaches and uses a logistic regression-based model for the final simulator because of its stability, interpretability, and practical suitability.

The model estimates trial success probability based on predefined design variables and allows users to explore how design changes affect predicted outcomes.

The final model was evaluated using ROC curve analysis and calibration analysis to assess both classification performance and probability reliability.

## Economic Analysis

The economic analysis uses a simplified cost estimation structure:

**Estimated Trial Cost = Trial Duration × Daily Trial Cost**

The platform then compares the estimated cost before and after AI-assisted optimization.

The goal is not to reproduce the exact real-world cost of each individual clinical trial, but to provide a consistent framework for comparing relative cost changes between traditional and AI-optimized design scenarios.

The ROI efficiency analysis assumes the same revenue before and after AI application, then compares whether reduced development cost improves the cost-to-return structure.

## Website Structure

The website consists of the following main sections:

- **Home**: Introduction to the project and research motivation
- **AI Model**: Interactive clinical trial success probability simulator
- **Economics**: Economic impact and cost-saving simulation
- **Research**: Explanation of the research process and methodology
- **About**: Project summary and background information

## Tech Stack

This project is implemented as a web-based prototype.

Technologies used or suitable for this project include:

- React
- JavaScript
- Python
- Machine learning model analysis
- Data visualization
- Vercel deployment

## Project Significance

This project demonstrates how AI can be used not only for medical diagnosis or drug discovery, but also for optimizing the structure of clinical trials themselves.

By combining predictive modeling with economic analysis, the platform presents clinical trial design as both a scientific and financial decision-making problem.

The project highlights the possibility that AI-assisted trial design could:

- Improve clinical trial efficiency
- Reduce unnecessary development costs
- Shorten trial timelines
- Support better resource allocation in pharmaceutical R&D
- Contribute to broader healthcare cost reduction

## Limitations

This project is a research prototype and should not be used as a real clinical decision-making system.

Key limitations include:

- The dataset is simplified for research and simulation purposes
- The model does not replace expert clinical judgment
- Real-world clinical trial outcomes depend on many biological, regulatory, and operational factors
- The cost model is standardized and does not fully represent all trial-specific expenses
- The platform is intended for educational and research demonstration purposes only

## Future Improvements

Future development could include:

- Expanding the dataset with more real-world clinical trial records
- Supporting additional diseases and trial phases
- Improving the prediction model with more advanced machine learning techniques
- Adding uncertainty estimates for model predictions
- Incorporating more detailed cost components
- Developing a more comprehensive decision-support dashboard for researchers

## Disclaimer

This platform is for educational and research demonstration purposes only.

It does not provide medical advice, clinical recommendations, or regulatory guidance.
