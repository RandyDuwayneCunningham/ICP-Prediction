# ICP Property Prediction Using Machine Learning

This repository contains the code and data for predicting physical properties of **Impact Polypropylene (ICP)** using machine learning models trained on industrially sourced data.

## 📌 Project Overview

Experimental determination of physical properties like **tensile modulus**, **flexural modulus**, and **impact strength** is time-consuming and delays real-time decisions in manufacturing environments. This project demonstrates the use of machine learning (ML) techniques to predict these properties using structural features measured via standard industrial methods.

## 🧪 Dataset

The dataset consists of **483 industrially validated ICP samples**, each with:
- Structural parameters:  
  - Melt Flow Rate (MFR)  
  - Ethylene Content (C2)  
  - Rubber Ethylene Content (RCC2)  
  - R21 (Amorphous fraction indicator)
- Physical property targets:  
  - Tensile Modulus  
  - Flexural Modulus  
  - Impact Strength

> **Note:** The structural parameters are derived using ISO methods, making the trained model transferable across different ICP production facilities.

## 🧠 ML Models Used

- **Linear Regression** – Used as a baseline for linear modeling.
- **Random Forest Regressor** – Selected for its ability to handle non-linearities, interpretability, and low computational cost.
- **Neural Network** – Tested for capturing complex patterns in structural-property relationships.

## 📊 Key Findings

- **Random Forest** performed best across all properties with R² values of:
  - 0.78 for Tensile Modulus
  - 0.75 for Flexural Modulus
  - 0.88 for Impact Strength
- **Feature reduction** revealed that only **MFR** and **R21** were required for accurate predictions, enabling faster, simpler deployment in real-world settings.

