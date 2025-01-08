Welcome to the world of Databricks! In this course, you will be introduced to the Databricks Lakehouse platform and understand how it modernizes data architecture using the new Lakehouse paradigm. You'll explore the foundational components of Databricks, including the UI, platform architecture, and workspace administration. Interactive exercises will guide you through SQL queries, platform features, and external system connections for efficient data management and seamless integration. Additionally, you'll delve into the Databricks Data Intelligence Platform, covering data management, compute capabilities, catalog management, and data ingestion. You'll also learn to use Databricks as a data warehousing solution for Business Intelligence (BI), leveraging SQL-optimized capabilities to create queries and analyze data.

✅ [Introduction to Databricks](https://github.com/janaom/databricks-learning/blob/main/introduction-to-databricks/README.md#introduction-to-databricks)

✅ [Data Intelligence Platform Fundamentals](https://github.com/janaom/databricks-learning/blob/main/introduction-to-databricks/README.md#data-intelligence-platform-fundamentals)

✅ Introduction to SQL in Databricks


# Introduction to Databricks

Discover how the Databricks Lakehouse platform modernizes data architecture using the new Lakehouse paradigm. Explore the foundational components of Databricks and their integration. Engage with the Databricks UI, platform architecture, and workspace administration. At the same time, practical exercises guide you through SQL queries, platform features, and external system connections, introducing you to the efficient data management and seamless integration Databricks can offer.

------------------------

## Databricks Architecture

![image](https://github.com/user-attachments/assets/6f6e7d8f-e34e-4aeb-a860-f92984e96f94)

In Databricks, the control plane and compute plane are distinct layers responsible for different aspects of the platform's operation:

- **Control Plane**: This is the management and orchestration layer. It handles user authentication, cluster management (starting, stopping, scaling), workspace administration, metadata management, and overall platform operations. Think of it as the "brains" of the operation. It's responsible for coordinating and monitoring the compute resources.

- **Compute Plane**: This is where the actual data processing happens. It consists of the worker nodes that execute Spark jobs and other computations. These are the clusters you create to run your code. The compute plane is responsible for the heavy lifting of data processing and analysis. Think of it as the "muscles" doing the work.

In short: The control plane manages the resources, while the compute plane uses those resources to perform computations. They work together seamlessly to provide the Databricks service.

## Administering a Databricks workspace

![image](https://github.com/user-attachments/assets/07aab8d2-8878-4b00-b7ab-21a7483602e6)

Which statement best reflects the difference between an Account Admin and a Workspace Admin?

- Account Admins have permissions to the entire account and back-end configurations, while Workspace Admins have permissions for the operations within a specific workspace.

# Data Intelligence Platform Fundamentals

Learn the key components of the Databricks Data Intelligence Platform and how it can enhance your analytical processes. Explore Databricks fundamentals for data management and compute capabilities. You will also cover data catalog management and data ingestion. Get your hands dirty with interactive exercises that will guide you through integrating datasets, setting permissions, and configuring clusters. 

## Data Intelligence Platform - Data

With Databricks, we recommend storing data in the Delta format.

![image](https://github.com/user-attachments/assets/8e70f0eb-f42c-4e0f-aafe-dd9dc39f37a9)

Once data has been stored, we need to manage how that data is accessed and governed. 

Unity Catalog provides a holistic governance layer on top of everything in the lakehouse.

![image](https://github.com/user-attachments/assets/0786ac8d-cdfa-4221-80f2-144b504d37ca)

![image](https://github.com/user-attachments/assets/2a754e1f-873f-4cf9-9212-3b85dd5c5e09)

What is one of the primary benefits of using the Catalog Explorer instead of your previous approach?

- Ability to see sample data for a particular table.


## Data Intelligence Platform - Compute

![image](https://github.com/user-attachments/assets/1b337d17-1af3-4d98-89de-6d38452e37b8)

![image](https://github.com/user-attachments/assets/ac95ab66-3ed4-4468-8e6f-1245c02b1e2b)

![image](https://github.com/user-attachments/assets/18a2e47d-16b7-4be6-b234-4e24d7887597)

![image](https://github.com/user-attachments/assets/ed888c48-4431-4017-972a-265c81b55e52)

## Node capabilities: Single vs. Multi

![image](https://github.com/user-attachments/assets/2753d5b7-4820-4f30-89e3-1a60bb095fdd)

## Configuring clusters

You have received various requests from your central IT group to reign in the kinds of clusters that can be created in Databricks.

The IT team will start implementing different cluster policies for the different groups using the Databricks platform. Since you lead your data engineering team, the IT team would like you to provide a list of configurations you need to complete your work.

Which of the following is not a valid cluster configuration in Databricks?

+ Cluster monthly budget (While you can use Databricks to track your costs spent on a particular cluster, you cannot specify a budget for how much the cluster will cost each month directly.)

# Introduction to SQL in Databricks

Use the Databricks Data Intelligence Platform as your data warehousing solution for your Business Intelligence (BI) use cases. Use the built-in SQL-optimized capabilities within Databricks to create queries and dashboards on your data.

## Data Intelligence Platform - Analytics

Options to interact with data in Databricks:

![image](https://github.com/user-attachments/assets/31e0ef38-7c4b-4af3-8930-a25234154e7a)

![image](https://github.com/user-attachments/assets/66eb5be8-f4a3-414a-8535-44ff635a55b8)

As you migrate your existing data pipelines into Databricks, your data engineering team wonders if they are selecting the correct language for development. While you don't want to refactor everything, you want to ensure the selected language is the best long-term selection for your problem, and that Databricks can support the required language.

Which of the following tasks would be supported in Databricks?

+ Creating a custom function for a business-specific calculation in Python
+ Joining two tables together in SQL
+ Performing advanced statistical techniques on your data

![image](https://github.com/user-attachments/assets/833b87a7-e843-4ec4-b44e-f2c67f9d6262)

## SQL in the Data Intelligence Platform

