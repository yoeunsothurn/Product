Explanation:
CreateTableExample Class:

Establishes a connection to MySQL using JDBC (DriverManager.getConnection).
Creates a Statement object to execute SQL queries (connection.createStatement()).
Defines a SQL CREATE TABLE statement (String sql = "CREATE TABLE ...").
Executes the SQL statement to create the Product table (statement.executeUpdate(sql)).
Closes the resources (statement and connection) in the finally block.
RetrieveProductsExample Class:

Establishes a connection to MySQL using JDBC (DriverManager.getConnection).
Creates a Statement object to execute SQL queries (connection.createStatement()).
Defines a SQL SELECT statement to retrieve all products from the Product table (String sql = "SELECT * FROM Product").
Executes the SQL query (statement.executeQuery(sql)), which returns a ResultSet.
Iterates through the ResultSet, retrieves each product's attributes (id, name, price_per_unit, active_for_sell), and prints them to the console.
Closes the resources (resultSet, statement, and connection) in the finally block.
Running the Application:
Ensure you have MySQL installed and running on your machine.
Replace JDBC_URL, USERNAME, and PASSWORD with your MySQL connection details.
Run CreateTableExample to create the Product table.
Run RetrieveProductsExample to retrieve and display all products from the Product table in the console.
