# DYNAMIC-PRICE-OPTIMISATION-ENGINE

Dynamic Price Optimization Engine


A machine learning-powered dynamic pricing system that analyzes demand, seasonality, and price elasticity to optimize product prices in near real-time. Built using LightGBM, PySpark, MLflow, FastAPI, and Docker, this project combines data processing, modeling, and deployment in a modular, production-ready setup.

# Overview


This engine predicts demand and suggests prices for multiple SKUs based on historical sales and product catalog data. It includes:

    Feature Engineering: Lag features, elasticity metrics, and demand indicators to improve forecast accuracy.

    Demand Forecasting: Trained LightGBM models using GridSearchCV for reliable predictions.

    Price Optimization: Combines demand signals and rule-based logic to suggest SKU-level prices.

    Real-Time API: Exposes predictions through a FastAPI server, containerized with Docker.

    Reproducible Pipelines: Built with PySpark, MLflow, and DVC for experiment tracking and versioning.

# Why This Approach

    LightGBM handles tabular data efficiently, supports nonlinear interactions, and scales well.

    Rule-based pricing logic ensures practical constraints, such as:

        Cost floors

        Competitor-based price caps

        Demand-driven adjustments (+/-5%)


This setup balances accuracy, interpretability, and real-world applicability. Future improvements could include constrained optimization for more precise pricing.

# Project Context


Inspired by a real-world client scenario, this project replicates a demand-driven pricing system while using synthetic data to preserve confidentiality. The system demonstrates full end-to-end ownership:

    Data simulation and preprocessing

    Feature engineering and modeling

    Modular pipelines for reproducibility

    API deployment and containerization


Some utilities (like dataset generation, FastAPI scaffolding, and testing scripts) were developed collaboratively with permission, while all core pipelines and modeling were independently implemented.

# Technical Stack

    Data Processing: PySpark, Pandas

    Modeling: LightGBM, GridSearchCV

    Tracking & Versioning: MLflow, DVC

    Deployment: FastAPI, Docker

    Other Tools: Git, CI/CD ready

# Key Takeaways

    Designed a modular, scalable system for dynamic pricing.

    Achieved real-time forecasting and price recommendations.

    Ensured reproducibility and version control for datasets and models.

    Developed an end-to-end pipeline demonstrating ownership and practical ML
