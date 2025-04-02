## 2A- Transformation on the Northwind Database

1. Import Northwind Dataset
   (http:services.odata.org/V3/Northwind/Northwind.svc/)

2. Transform Data - Power BI Query Editor

3. Select the Categories table -> Choose
   Columns -> **CategoryID, CategoryName and Description**

4. Select the Customers table -> Choose
   Columns -> **CustomerID and ContactName**

5. Select the Orders table -> Choose
   Columns -> **OrderID, OrderDate, ShipCity and ShipCountry**

6. Select the Products table -> Choose
   Columns -> **ProductID, ProductName and CategoryID**

7. Select the Order_Details -> . Expand the **Order column** and select
   CustomerID. **Rename** the column **Orders.CustomerID to CustomerID**

8. Add Column ribbon, click on Custom Column -> LineTotal = [UnitPrice] \* [Quantity]

9. Close & Apply.

10. Click on the Modelling tab and select Manage relationships.

11. Add Relationship -> **Orders_Details.CustomerID** to **Customers.CustomerID** -> many to one
