# Databricks Concepts

This course guides you from start to finish on how the Databricks Lakehouse Platform provides a single, scalable, and performant platform for your data processes. As you work through a real-world dataset, you will learn how to accomplish a variety of tasks within the Databricks platform. Throughout this course, you will learn about and practice the different features of the Databricks Lakehouse platform and see how they can be applied to different data use cases

--------------------

  ✅  [Welcome to Databricks](https://github.com/janaom/databricks-learning/blob/main/databricks-concepts/README.md#welcome-to-databricks)

  ✅  [Data Engineering](https://github.com/janaom/databricks-learning/blob/main/databricks-concepts/README.md#data-engineering)

  ✅  [Databricks SQL and Data Warehousing](https://github.com/janaom/databricks-learning/blob/main/databricks-concepts/README.md#databricks-sql-and-data-warehousing)

  ✅  [Databricks for Large-scale Applications and Machine Learning](https://github.com/janaom/databricks-learning/blob/main/databricks-concepts/README.md#databricks-for-large-scale-applications-and-machine-learning)

------------------------

# Welcome to Databricks

Learn about the new lakehouse paradigm for your cloud data strategy and how the Databricks Lakehouse platform can modernize your data architecture. Understand the foundational components of the Databricks platform and how they all fit together.

## Introduction to the Databricks Lakehouse Platform

![image](https://github.com/user-attachments/assets/77cf0dd3-ff55-4f5d-a958-c233eff0e9a1)

![image](https://github.com/user-attachments/assets/b16eaaef-adb8-4d62-afb0-4af8a4ad624c)

![image](https://github.com/user-attachments/assets/72b2d913-2af7-4920-bba3-29faa41d1166)

![image](https://github.com/user-attachments/assets/60b0a9b8-a363-4d29-9510-207e81f781dd)

![image](https://github.com/user-attachments/assets/f71a526b-4940-4faf-8515-30426423b56d)

![image](https://github.com/user-attachments/assets/9ce1a101-90ab-4a39-b0d5-1a6e3e750d72)

Why Delta?

As you develop your future-state architecture, you have started to think about how to store your organization's data. You know you want to store data in a data lake and have heard a lot about the Delta Lake table format.

Which of the following are the benefits of storing data in the Delta table format? Select all that apply.

+ Fully ACID-compliant transactions
+ Unified batch and streaming data sources
+ Time travel and table history

## Control Plane vs. Data Plane

Which of the following is true regarding the relationship between the Databricks Control Plane and the customer Data Plane?

+ User interactions with the Databricks platform exist within the Control Plane, and is responsible for tasks such as launching clusters and initiating jobs.
+ The Data Plane is where customers store their data in the data lake, ensuring better data security.

![image](https://github.com/user-attachments/assets/ad895e14-e527-4c6e-a83e-b78d47cca900)


# Data Engineering

Learn how to process, transform, and clean your data using Databricks functionality. Practice using capabilities such as the Delta storage format, Delta Live Tables, and Workflows together to create an end-to-end data pipeline.

## Getting started with Databricks

![image](https://github.com/user-attachments/assets/53bf1a26-edeb-4abd-a808-b68c5d2f9ab7)

![image](https://github.com/user-attachments/assets/b0ecc687-1c70-4d26-a08a-636a76bfa2cc)

## Data Engineering foundations in Databricks

![image](https://github.com/user-attachments/assets/3a59c1bc-5795-4f8d-9cca-2a55b8f18825)

![image](https://github.com/user-attachments/assets/f3c48ec3-c144-4135-ae5c-4a26adb05957)

## Data orchestration in Databricks

In the Databricks platform, data engineers can orchestrate their data using tools lumped into an offering called Databricks Workflows, where you can automate every task you can achieve in Databricks with built-in capabilities at no additional cost. Here is a diagram showing a high-level potential pipeline you could orchestrate in Databricks Workflows. This pipeline reads in two different datasets (one batch, one streaming) and uses Delta Live Tables to process and eventually join these datasets. From there, different data persona could do further analytics processes, such as ML model training and dashboard serving. 

Databricks Workflows is designed to orchestrate and automate nearly everything you can do with the Databricks platform, so what exactly can we include in our Workflows? If you are a data engineer or data scientist, you will be able to automate all of your programmatic work like Databricks notebooks or Delta Live Table pipelines. Users can also include external .jar files, Spark submit jobs or Java applications. Databricks also allows you to include external orchestration tools in Workflows. For example, dbt is used to schedule and test SQL queries. As a data analyst, you can automatically include any queries, dashboards, or alerts as part of a Workflow.

Databricks Jobs are the core of Workflows and define a particular step in the overall Workflow pipeline. For example, a single Job could join order and customer datasets together. In Databricks, there are multiple ways to create a Job. In the UI, users can create a job quickly, no matter where they are. Users can create a job in the context of a notebook or go to the Workflows area of the UI, where you can create and manage your Workflows and Jobs together. Here is a screen shot of the pop-up box to create a Job directly from the context of a notebook. 

![image](https://github.com/user-attachments/assets/794aa18a-bf62-44c7-9604-74fdf28b86d6)

![image](https://github.com/user-attachments/assets/344b2226-fe4b-4eda-b9ed-e4742e8d5cf8)

![image](https://github.com/user-attachments/assets/53471603-aad6-44c0-9b27-7d2f3957a9ea)

The correct sequence to create an automated data pipeline

![image](https://github.com/user-attachments/assets/e0c51e4b-172f-4792-a3e1-41195735500a)

# Databricks SQL and Data Warehousing

Use the Databricks Lakehouse platform as your data warehousing solution for your Business Intelligence (BI) use cases. Use the built-in SQL-optimized capabilities within Databricks to create queries and dashboards on your data.

## Getting started with Databricks SQL

![image](https://github.com/user-attachments/assets/d2b30436-63e7-45a0-8337-e89e6a242507)

![image](https://github.com/user-attachments/assets/156521c8-43d5-48f0-83cc-e4e4381bc5c6)

![image](https://github.com/user-attachments/assets/1a9f8d89-2e1f-40f4-908c-412b27c0c3da)

### Choosing your SQL warehouse

You are starting to query some of Sierra Publishing's book sale data and want to ensure you have the right kind of SQL warehouse for what you need. You want to make sure you have the latest features that Databricks has put out there. Your users are also used to quickly accessing the data behind their reports and don't want to wait for the warehouse to spin up too long.

What kind of SQL warehouse should you create?

+ Serverless

# Databricks for Large-scale Applications and Machine Learning

Use Databricks to manage your Machine Learning pipelines with managed MLFlow. Follow the model development lifecycle from end-to-end with the Feature Store, Model Registry, and Model Serving Endpoints to create a robust MLOps platform in the lakehouse.

## Overview of Lakehouse AI

![image](https://github.com/user-attachments/assets/c0fb3c7e-d5b7-4b84-9e72-62d069cea598)

The beginning of the MLOps process falls into DataOps, which involves getting data ready for any kind of machine learning application. This starts by integrating data from different sources into the Delta lake, which can use the AutoLoader capability. Then, we want to transform those data tables into a more usable, clean format, which often can be completed with Delta Live Tables. Finally, data scientists need to create tables of different features to feed into the model they choose, which uses the Feature Store capability in the platform. 

![image](https://github.com/user-attachments/assets/776f3045-2ec5-4ce1-b6da-1bb9febdbc01)

After data has been processed correctly, a data scientist can start developing a machine learning model. They will begin by developing and training a model, usually done in Databricks Notebooks or in a local IDE. Some users are looking for a pre-defined model template that can utilize Databricks AutoML to generate a baseline model. Throughout the process, data scientists must track metrics and parameters to understand their model performance using the MLFlow framework. Once the model is developed, the model must be centralized so that users can consume and use the model, which uses the Databricks Model Registry. 

![image](https://github.com/user-attachments/assets/210d0143-aff5-432b-8e40-d1cc978c7240)

At the end of the MLOps process, we have DevOps, which is all about getting the developed models into a production capacity. Throughout the development process, and especially once a model is ready for deployment, access must be governed securely, which can utilize Unity Catalog in the Databricks environment. As models are tuned over time, data scientists need to control which version of a model is in production and which is in a testing environment, which can be controlled in the Model Registry. Finally, the model is ready for deployment, which can be done directly from Databricks Serving Endpoints. 

![image](https://github.com/user-attachments/assets/728cc46a-24b9-4e75-8722-2d4dc0a5ca11)

Databricks helps streamline the featurization process with the Feature Store, a centralized storage specifically for feature tables. With the Feature Store, you can discover and re-use feature tables for your different models and see upstream and downstream lineage from that feature table. Here, we can quickly create a feature table based on an existing DataFrame we created for our features. Now, any model in the future can reference our feature table, which expedites the development process. 

![image](https://github.com/user-attachments/assets/c3811e0b-1792-466c-aa0e-d4040babea54)

Each code block represents a different cell in a Databricks notebook. Put each code block in the correct order to complete your task.

![image](https://github.com/user-attachments/assets/fcf42af6-4b0e-459f-a29a-1dbb452fd880)

## Model training with MLFlow in Databricks

Before diving into Databricks-specific functionality, let's talk about scaling up machine learning workloads. Single-node machine learning is the classical approach for these workloads, as they will only use a single machine (for example, your laptop) to train a model. This is a great approach for experimenting and testing, as the setup is easy and quick. However, these models don't typically work well in a production setting, as they cannot scale how we need them to. The most popular example of these kinds of models are from the scikit-learn library. Most organizations are looking at moving into multi-node machine learning, which uses multiple compute resources (like a Databricks cluster) to train a model. These are much better for production workloads. While they require a slightly harder setup, they are much easier to maintain over time, as they are very scalable. This is where frameworks like Spark ML can be hugely helpful. 

![image](https://github.com/user-attachments/assets/feabde6a-bb74-4698-97c4-5bdf76e2517e)

If you aren't very comfortable programming your own machine learning pipeline or just want a good foundation, you will benefit from the AutoML capability in Databricks. AutoML is a Glass Box approach to machine learning. Many other tools can automatically create a machine-learning model, but they don't provide much visibility into what is happening under the hood. With Databricks AutoML, the platform uses the most popular open-source libraries and can create a model that best predicts what you want it to predict based on your UI selections. To take it a step further, AutoML generates a notebook with the required code to reproduce, audit, or optimize the code for that model, so you know exactly what happened. 

![image](https://github.com/user-attachments/assets/45ac7d91-a299-4cae-926b-782cfb1a595e)


