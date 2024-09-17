# AWS-Part2

___

# Project Description: Descriptive Analysis of 311 Service Center
This assignment is continuation for improvement of the [AWS-Part1-Venkat](https://venkat-ramana-reddy-bhoom-reddy.github.io/AWS-Part1-Venkat/) project using the datasets taken from  website [City of Vancouver Open Data Portal](https://opendata.vancouver.ca/explore/dataset/3-1-1-service-requests/information/?disjunctive.department&disjunctive.service_request_type&disjunctive.status&disjunctive.closure_reason&disjunctive.local_area&disjunctive.channel). This project concentrates on details of protection, governance and monitoring of DAP.

## Project Title: Data Protection, Governance, & Monitoring for DAP
This project concentrates on details of protection, governance and monitoring of DAP. As these 3 are vital thing that must be ensured for all the current project. Lack of any of these three aspects would result in the project execution lacking or even failure of the project. We will see how below:
## Project Objective:
* Data Protection design and implementation.
* Data Governance design and implementation.
* Data Monitoring design and implementation.
## Datasets
* The Dataset used is taken from [City of Vancouver Open Data Portal](https://opendata.vancouver.ca/explore/dataset/3-1-1-service-requests/information/?disjunctive.department&disjunctive.service_request_type&disjunctive.status&disjunctive.closure_reason&disjunctive.local_area&disjunctive.channel) for the category of "3-1-1 service request metrics"<br>
[cumulative_3-1-1-service-requests_2023_open.xlsx](https://github.com/user-attachments/files/17021197/cumulative_3-1-1-service-requests_2023_open.xlsx)
* This dataset contains location information such as address or intersection where service was requested and the local area corresponding to the case (incident) location.
## Methodology:
* The process involves 3 different steps explained in detail below:
### Step 15: Data Protection
* This **Data Protection** providing protectio to data in many ways like encryption or access granting or other methods.<br>
![fig10](https://github.com/user-attachments/assets/9381e20a-f07e-48d5-8826-3f701e3cb7e1)
* The above image shows how I created a KMS key for encryption and decryption of data.<br>
![appx005](https://github.com/user-attachments/assets/c75a77ce-b627-4ebd-9e94-269134c42a24)
* The above image shows configuration details of the KMS key.<br>
![fig11](https://github.com/user-attachments/assets/6a5d1852-d9c0-44b2-ad4f-12beb04ce247)
 The above image shows the changes made to enable encryption and bucket versioning for S3 bucket.<br>
![fig13](https://github.com/user-attachments/assets/d56cc677-a0f4-454f-b7c1-56ea37bdb434)
* The above image shows the changes made to enable replication rule for S3 bcket.<br>
![fig12](https://github.com/user-attachments/assets/5fdf14ad-895c-47ef-8cf4-6c6193a9416d)
* The above image shows the changes made to enable encryption and bucket versioning for S3 backp bucket.
### Step 16: Data Governance
* Data governance refers to the policies, standards, and practices for managing and using data in a way that aligns with organizational goals and regulatory requirements to ensures the quality, integrity, and security of data across its lifecycle.
![fig24](https://github.com/user-attachments/assets/ecde8087-864c-48ea-9e63-4e776e7c80dc)
* The above image shows the trusted folder created in S3 bucket.<br>
![fig25](https://github.com/user-attachments/assets/e03bcc60-862c-4676-af9c-7ebd4e9cb3de)
* The above image shows the ETL designed to mask sensitive data and store it in trusted folder.<br>
![appx015-1](https://github.com/user-attachments/assets/c165de7b-8811-437e-affa-5b5b5cd9b1a6)
* The above image shows the results of eTL design.<br>
![appx017](https://github.com/user-attachments/assets/092011dd-cf8b-41e9-b0d7-6240e00bce44)
* The above image shows the workflow designed.<br>
![appx015-2](https://github.com/user-attachments/assets/160d8434-e60c-4e80-80e8-82b8a36c1305)
* The above image shows the job run details.<br>
![appx018](https://github.com/user-attachments/assets/33a6ab12-36bf-4dfa-bd7c-d19bfd8aa381)
* The above image shows the Data Quality details.<br>
![appx016](https://github.com/user-attachments/assets/837db789-1ec6-4641-8b74-f0dd8097461e)
* The above image shows the job scheduling.<br>
### Step 17: Data Monitoring
* Data monitoring involves continuously tracking data usage and access to ensure compliance with governance policies, detect potential breaches, and maintain data integrity.
![appx025](https://github.com/user-attachments/assets/ff19d665-842d-4c52-8f49-21fc963c16d8)
* The above image shows alarm information.<br>
![fig36](https://github.com/user-attachments/assets/c580daf2-306c-4429-9550-22187d9afada)
* The above image shows the dashboard.<br>
![fig37](https://github.com/user-attachments/assets/2d64ad93-8bbd-46f4-a124-0ab8ad64dbfc)
* The above image shows the cloud trail created.<br>
![fig38](https://github.com/user-attachments/assets/c28ed257-cd1a-439b-a7f0-2aaa06c38ce3)
* The above image shows the cloud trail outcome stored in S3 buckets.<br>
