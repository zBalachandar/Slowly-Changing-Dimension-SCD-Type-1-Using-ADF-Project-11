# Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11
In this project, I discussed about Slowly changing Dimension Type1 using mapping data flows in Azure Data Factory (ADF).
<div align="center">
  <a href="#">
    <img src="https://github.com/zBalachandar/Azure-data-factory-Real-time-Transformation-end-to-end-Pipeline-Project-10/blob/531ef59f65fb8326a86e172d8802420763c92ad9/Assets/AZURE%20portal%20ov.png" alt="Banner" width="720">
  </a>

  <div id="user-content-toc">
    <ul>
      <summary><h1 style="display: inline-block;"> End to End Data-Pipeline-Project </h1></summary>
    </ul>
  </div>
  
  <p>Data Pipeline using Azure DataFactory</p>
</div>
<br>

### 💾 Dataset
Dataset : 
<br>
<div>
  SQL script:
➖➖➖➖
CREATE TABLE employee
(
    employee_id INT,
    FirstName NVARCHAR(128),
    salary INT,
    location NVARCHAR(128)
)

INSERT INTO EMPLOYEE VALUES(1,'manish',10000,'india')
INSERT INTO EMPLOYEE VALUES(2,'NEHA',5000,'india')
INSERT INTO EMPLOYEE VALUES(4,'SURYA',5000,'UK')
</div>

</br>
### Business Requirement.
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/Business%20requirements.jpg)

### Design and Development of pipeline:
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/pipeline%20showcase.png)

### Project steps to follow: 
what we have covered in this project:

- We have Covered End to End ADF Pipeline Project 
- Developed the Data Pipeline according to the business requirement


<a name="data-transformation"></a>
### ⚙️ Data Pipeline
 Create the resources for Data pipeline and processing using AZURE DATA FACTORY.
![image](https://github.com/zBalachandar/Azure-data-factory-Real-time-Transformation-end-to-end-Pipeline-Project-10/blob/531ef59f65fb8326a86e172d8802420763c92ad9/Assets/AZURE%20portal%20ov.png)

Azure SQL Server:
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/ASQL%20db%20DEPLOYMENT.png)
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/sql%20query%20-table%20created.png)
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/sql%20query%20-table%20view.png)
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/sql%20query%20-table%20view%201.png)

Create the Azure Data Factory:
![image](https://github.com/zBalachandar/Azure-data-factory-Real-time-Transformation-end-to-end-Pipeline-Project-10/blob/531ef59f65fb8326a86e172d8802420763c92ad9/Assets/Datafactory%20ov.png)

Create Source point: 
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/pipeline%20showcase.png)

![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/dataflow%20pipeline%20s1.png)

![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/dataflow%20pipeline%20s1.png)

Dataflow :
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/pipeline%20running%20succesfully%20g1.png)
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/Factory%20config%20the%20csv.png)

 Debug:
![image](https://github.com/zBalachandar/Azure-data-factory-Real-time-Transformation-end-to-end-Pipeline-Project-10/blob/93b868a93a4f407a27143a8797420ce942ebc83d/Assets/Dataflow%20debug.png)

Data Preview:
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/dataflow%20pipeline%20s1.png)

pipeline 1: 
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/running%20tigger%20the%20pipelineg1.png)

pipeline 2,3:
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/dataflow%20pipeline%203.png)

Publish all the Activities and dataflow:
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/pipeline%20showcase.png)

Run pipelines:
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/pipeline%20success%201.png)
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/pipeline%20running%20succesfully%20g1.png)

Desired Output - SQL SCD operation :
![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/RESULT%20G1%20SUCCESSP1.png)

![image](https://github.com/zBalachandar/Slowly-Changing-Dimension-SCD-Type-1-Using-ADF-Project-11/blob/0a0d90c7851705963c5f756fc0b997eb3cfd7f3d/Assets/RESULT%20G1%20SUCCESSP2%20sql.png)

### 🛠️ Technologies Used

- **Data Pipeline**: Azure Data Factory
- **Data Loading**: Azure SQL Server, Database.

<a name="credits"></a>
## 📋 Credits

- This Project is inspired by the video of the [YouTube Channel "Learn by doing it"](https://www.youtube.com/watch?v=pMqnvXgPKlI&list=PLOlK8ytA0MghGmAAT8W2u7VYmICdzeU5t&index=1&t=96s)  

<a name="contact"></a>
## 📨 Contact Me

[LinkedIn](https://www.linkedin.com/in/balachandars2022/) •
[Gmail](balachandar2014elu@gmail.com)  •

