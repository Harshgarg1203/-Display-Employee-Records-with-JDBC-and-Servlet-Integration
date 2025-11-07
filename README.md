# Display Employee Records with JDBC and Servlet Integration

## 🎯 Objective
To create a Java Servlet that connects to a MySQL database using JDBC and displays a list of employees with a search feature.

## 📂 Project Structure
```
EmployeeDisplayApp/
├── src/com/example/servlet/EmployeeServlet.java
├── WebContent/index.html
└── WebContent/WEB-INF/web.xml
```

## ⚙️ Setup Instructions
1. Create a MySQL database named `companydb`.
2. Run the following SQL command:
   ```sql
   CREATE TABLE Employee (
       EmpID INT PRIMARY KEY,
       Name VARCHAR(50),
       Salary DOUBLE
   );

   INSERT INTO Employee VALUES (101, 'Alice', 60000), (102, 'Bob', 55000), (103, 'Charlie', 70000);
   ```
3. Update database credentials in `EmployeeServlet.java`.
4. Import the project into Eclipse/NetBeans.
5. Deploy on Apache Tomcat and open:
   ```
   http://localhost:8080/EmployeeDisplayApp/
   ```

## 🧠 Concepts Demonstrated
- JDBC connection handling
- SQL query execution
- Dynamic HTML table generation
- Servlet request parameter handling
