# Databricks Concepts

This course guides you from start to finish on how the Databricks Lakehouse Platform provides a single, scalable, and performant platform for your data processes. As you work through a real-world dataset, you will learn how to accomplish a variety of tasks within the Databricks platform. Throughout this course, you will learn about and practice the different features of the Databricks Lakehouse platform and see how they can be applied to different data use cases

--------------------

  ✅  [Welcome to Databricks](https://github.com/janaom/databricks-learning/blob/main/databricks-concepts/README.md#welcome-to-databricks)

  ✅  [Data Engineering](https://github.com/janaom/databricks-learning/blob/main/databricks-concepts/README.md#data-engineering)

  ✅  [Databricks SQL and Data Warehousing](https://github.com/janaom/databricks-learning/blob/main/databricks-concepts/README.md#databricks-sql-and-data-warehousing)

  ✅  Databricks for Large-scale Applications and Machine Learning

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


