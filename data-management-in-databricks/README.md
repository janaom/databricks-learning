# Data Management in Databricks

Ready to level up your Databricks skills? In this course, you’ll master Data Management skills in Databricks, utilizing Delta Lake features like ACID transactions, schema enforcement, and time travel for rock-solid data management. Dive into creating and managing tables and temp views to streamline workflows. Then, explore Databricks’ Data Explorer to preview datasets, assign table ownership, and protect sensitive data with top-notch security practices. Whether crafting reusable queries or managing Personally Identifiable Information (PII), this course has you covered with hands-on exercises and practical strategies to keep your data secure, accessible, and optimized for any scenario.

✅ [Introduction to Delta Lake](https://github.com/janaom/databricks-learning/blob/main/data-management-in-databricks/README.md#introduction-to-delta-lake)

✅ [Working with Tables in Databricks](https://github.com/janaom/databricks-learning/blob/main/data-management-in-databricks/README.md#working-with-tables-in-databricks)

✅ [Data Exploration and Security](https://github.com/janaom/databricks-learning/blob/main/data-management-in-databricks/README.md#data-exploration-and-security)

----------------------
# Introduction to Delta Lake

This chapter explores table management in Databricks, focusing on managed vs. unmanaged tables and how they handle storage and lifecycle. You'll learn to create and refresh persistent views and dive into Delta Lake features like ACID transactions, schema enforcement, and time travel for reliable data management. You will also gain a deeper look into the mechanics of data organization and access within Databricks.

## Managing data in Delta Lake

![image](https://github.com/user-attachments/assets/1464e2aa-c3c4-4f5f-b7b6-03f310b98f3b)

![image](https://github.com/user-attachments/assets/55e6491e-1a53-4523-8bf6-af5fe0f430a1)


## Persistence and scope of tables

![image](https://github.com/user-attachments/assets/60519cff-c72f-401d-b2ce-9b9faeeaae5c)

![image](https://github.com/user-attachments/assets/2f4eaec6-2545-4c60-8488-5c6c42870940)

## Creating unmanaged tables

![image](https://github.com/user-attachments/assets/1f0c766f-56fc-4f9e-bff3-7738f032b99d)

# Working with Tables in Databricks

This chapter delves into creating and managing views and temp views in Databricks. You'll explore how persistent views save query logic for reuse across sessions, while temp views are suited for quick, session-specific tasks. The discussion also highlights practical scenarios where each type can enhance efficiency and streamline data handling.

## Views and Temp views

![image](https://github.com/user-attachments/assets/8fc6d4ab-3f7d-4aad-8388-e33bcb3451bc)

![image](https://github.com/user-attachments/assets/e917bb85-cd52-4b73-979e-79b11f692a62)

![image](https://github.com/user-attachments/assets/2a0eabcc-d891-430c-a159-376d01f6a43d)

![image](https://github.com/user-attachments/assets/27a49cf2-fe66-4344-ab9c-ae5faa5f2073)

Temp views are temporary objects that are only available for the current session. They're ideal for ad-hoc analysis or staging intermediate data during a pipeline. Let's create a temp view called temp_medical_records. In the SQL editor, we can type the following command.: Once the command is ready, we run it and notice the confirmation. This temp view behaves like a regular view, it only exists for the current session. If you close the session, it will be automatically dropped.

![image](https://github.com/user-attachments/assets/2b73b119-24ee-46d9-9c28-aae6321afb10)

In summary, use persistent views when you reuse query logic across sessions and choose temp views for quick, temporary operations that won't extend beyond the current session.

![image](https://github.com/user-attachments/assets/ba13aff8-73a6-476d-8244-6647df798959)

![image](https://github.com/user-attachments/assets/1c187f9b-7a9b-4897-976b-504444c2f797)

![image](https://github.com/user-attachments/assets/228bcb8b-b5e4-4687-861f-13fc3ddb98d2)

# Data Exploration and Security

In the final chapter, you’ll explore how to use Data Explorer to preview, analyze, and secure datasets. The content covers table ownership, responsibilities, and governance best practices. It also dives into managing access rights and securely handling Personally Identifiable Information (PII) with compliance-focused strategies and practical exercises.

## Managing access and understanding PII

In addition, understanding the implications of different access levels is crucial for effective data management. For example, granting read-only access is suitable for general users who only need to view data. In contrast, full access should be reserved for key personnel responsible for data updates and maintenance. Think of it like a museum exhibit: visitors can observe the displays, but only curators and staff are allowed to handle or modify the exhibits - Databricks' access control functions similarly to protect and maintain data integrity. 

Introducing Personally Identifiable Information, or PII, is important, but what is it? PII includes any data that can identify an individual, such as names, social security numbers, or medical records. Handling PII requires strict adherence to privacy laws and regulations, particularly in healthcare, finance, and government industries, where protecting sensitive data is vital. Proper handling of PII is not merely a best practice - it's a legal necessity enforced by regulations like GDPR and HIPAA. These laws dictate how PII must be stored, accessed, and shared to protect individuals' privacy and prevent data breaches that could lead to identity theft, financial loss, and other serious issues. 

![image](https://github.com/user-attachments/assets/fbbeee40-9376-48dd-8b9c-cdda75a77fb5)

![image](https://github.com/user-attachments/assets/222f4d64-8099-429d-ae45-ccfdc97e4c75)

![image](https://github.com/user-attachments/assets/d4924e90-42dc-4f45-b7db-e40c2806ffa5)


