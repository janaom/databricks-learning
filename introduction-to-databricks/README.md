Welcome to the world of Databricks! In this course, you will be introduced to the Databricks Lakehouse platform and understand how it modernizes data architecture using the new Lakehouse paradigm. You'll explore the foundational components of Databricks, including the UI, platform architecture, and workspace administration. Interactive exercises will guide you through SQL queries, platform features, and external system connections for efficient data management and seamless integration. Additionally, you'll delve into the Databricks Data Intelligence Platform, covering data management, compute capabilities, catalog management, and data ingestion. You'll also learn to use Databricks as a data warehousing solution for Business Intelligence (BI), leveraging SQL-optimized capabilities to create queries and analyze data.

✅ [Introduction to Databricks](https://github.com/janaom/databricks-learning/blob/main/introduction-to-databricks/README.md#introduction-to-databricks)

✅ Data Intelligence Platform Fundamentals

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

## Data Intelligence Platform - Data

With Databricks, we recommend storing data in the Delta format.

![image](https://github.com/user-attachments/assets/8e70f0eb-f42c-4e0f-aafe-dd9dc39f37a9)

Once data has been stored, we need to manage how that data is accessed and governed. 

Unity Catalog provides a holistic governance layer on top of everything in the lakehouse.

![image](https://github.com/user-attachments/assets/0786ac8d-cdfa-4221-80f2-144b504d37ca)

![image](https://github.com/user-attachments/assets/2a754e1f-873f-4cf9-9212-3b85dd5c5e09)

