#### Database-Implementation

##### Project Description  
Built a database for a consulting firm. Create SQL queries to answer client maintenance and employee training questions. 

##### Model Description      
In Homer Consulting each employee is assigned to (employed by) a specific department.   
The company runs projects for external clients. Information on both current clients as well as potential clients is kept.
Each project has several employees working on (assigned to) the project. Newly hired employees are not assigned to any project for the first few months and may be trained internally or by attending a formal workshop.
Homer Consulting maintains a list of desired skills. Each employee may take the same training more that once since some of the skills might need to be updated or renewed.  
  
##### Content 
* Create Table  
* Insert Value  
* Develop Query  
* Generate report   

##### Schema: 
| Table    | Field   |
| ---------| ------| 
| **SKILL** | (`Code`, Description) |
| **TRAINING** | (`Train_Num`, Code@, Emp_Num@, Date_Acquired, Name, Comments) |
| **DEPARTMENT** | (`Dept_Code`, Name, Location, Phone, Manager_ID@) |
| **EMPLOYEE** | (`Emp_Num`, Emp_Last, Emp_First, DOB, Hire_Date, Super_ID@, Dept_Code@) |
| **CLIENT** | (`Client_ID`, Name, Street, City, State, Zip_Code, Industry, Web_Address, Phone, Contact_Name) |
| **PROJECT** | (`Proj_Number`, Name, Start_Date, Total_Cost, Dept_Code@, Client_ID@) |
| **ASSIGNMENT** | (`Assign_Num`, Proj_Number@, Emp_Num@, Date_Assigned, Date_Ended, Hours_Used) | 
