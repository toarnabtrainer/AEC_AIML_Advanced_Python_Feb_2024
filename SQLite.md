# SQLite Database

<hr>

### What is SQLite Database?
SQLite is a popular open-source relational database management system (RDBMS) that is widely used in applications that require a local data store. It is a software library that provides a lightweight disk-based database that doesn't require a separate server process and allows for self-contained, zero-configuration installation.

SQLite is ACID-compliant, which means that it guarantees the reliability and consistency of data even in the presence of hardware or software failures. It supports a wide range of standard SQL features, including transactions, indexes, views, triggers, and stored procedures, making it a powerful tool for managing and querying data.

SQLite is used in a variety of applications, including web browsers, mobile devices, desktop applications, and embedded systems. It is widely supported and has bindings for many programming languages, including Python, Java, C++, and Ruby, making it easy to integrate into different types of software applications. Because it is a lightweight and fast database system, it is often used in scenarios where high performance and low overhead are critical factors.

<hr>

### Features of SQLite
SQLite is a powerful and versatile database system that has a number of features that make it an attractive choice for many different types of applications. Some of the key features of SQLite include:

* **Lightweight and fast:** SQLite is a small, self-contained database engine that is optimized for performance and low memory usage. It doesn't require a separate server process or configuration, making it easy to deploy and use in a wide range of applications.

* **ACID-compliant:** SQLite is ACID-compliant, which means that it ensures the reliability and consistency of data, even in the presence of hardware or software failures. It supports atomic transactions, rollbacks, and other features that make it suitable for mission-critical applications.

* **Cross-platform:** SQLite is available on a wide range of platforms, including Windows, macOS, Linux, iOS, and Android. It also supports a range of programming languages, including Python, Java, C++, and Ruby, making it easy to integrate into many different types of applications.

* **Wide range of SQL features:** SQLite supports a broad range of SQL features, including complex queries, indexes, views, triggers, and stored procedures. It also has a powerful SQL query optimizer that can improve performance and reduce the amount of data that needs to be read from disk.

* **Flexible data types:** SQLite supports a range of data types, including integers, floating-point numbers, strings, and dates, as well as BLOBs (binary large objects) that can store images, audio files, and other binary data.

* **Embeddable:** SQLite can be embedded into other applications as a library, making it an attractive choice for software developers who need a local data store for their applications.

* **Public domain:** SQLite is released into the public domain, which means that it can be used, modified, and distributed without any restrictions. This makes it a popular choice for open-source projects and other applications that require a free and open-source database system.

<hr>

### Application of SQLite
SQLite is a versatile database system that can be used in a wide range of applications, including:

* **Mobile apps:** SQLite is widely used in mobile app development, particularly for Android and iOS platforms. It provides a lightweight and fast data storage solution that can be easily integrated into mobile apps.

* **Web browsers:** Many web browsers, including Firefox, Chrome, and Safari, use SQLite as a data storage mechanism for things like bookmarks, history, and other user data.

* **Desktop apps:** SQLite can be used as a local database for desktop applications, particularly those that require a small and fast data store. It can be easily integrated into applications written in a range of programming languages, including Python, Java, and C++.

* **Embedded systems:** SQLite can be embedded into a wide range of embedded systems, including IoT devices, medical devices, and automotive systems. It provides a fast and reliable data storage solution that can operate in resource-constrained environments.

* **Data analysis:** SQLite can be used as a lightweight data analysis tool for small datasets. It supports complex SQL queries and provides a range of tools for data analysis, including aggregations, grouping, and sorting.

* **Education:** SQLite is often used as a teaching tool for database systems and SQL. Its small size and ease of use make it an attractive choice for educators who want to introduce students to database concepts without the complexity of a full-featured database system.

Overall, SQLite is a versatile and powerful database system that can be used in a wide range of applications, from mobile apps to embedded systems to data analysis. Its lightweight and fast design, coupled with its broad support for SQL features, make it an attractive choice for many different types of applications.

<hr>

### SQLite in Python
SQLite is well-suited for use in Python applications because it is a lightweight database system that is easy to use and requires minimal setup. Python includes a built-in module called sqlite3 that provides a simple and efficient way to interact with SQLite databases from Python code.

Here is a brief example of how to use SQLite in Python:

<pre>
import sqlite3

# Connect to the database
conn = sqlite3.connect('example.db')

# Create a table
conn.execute('''CREATE TABLE IF NOT EXISTS users (
                id INTEGER PRIMARY KEY,
                name TEXT NOT NULL,
                age INTEGER)''')

# Insert some data
conn.execute("INSERT INTO users (name, age) VALUES ('Alice', 30)")
conn.execute("INSERT INTO users (name, age) VALUES ('Bob', 25)")

# Retrieve data
cursor = conn.execute("SELECT * FROM users")
for row in cursor:
    print(row)

# Close the database connection
conn.close()
</pre>

In this example, we first import the sqlite3 module and use the connect() method to create a connection to an SQLite database file called example.db. We then use SQL statements to create a table called users, insert some data into it, and retrieve all the data using a SELECT statement. Finally, we close the database connection using the close() method.

The sqlite3 module provides a convenient way to interact with SQLite databases from Python code, and it supports a wide range of SQL features, including transactions, indexes, views, and more.

<hr>

<pre>
Content of the dataset file name 'emp_data.csv'

1001,Dhiman,Kolkata,39000
1002,Anupam,Kolkata,25000
1003,Subham,Mumbai,36000
1004,Dinesh,Chennai,28000
1005,Kakali,Mumbai,25000
1006,Bimal,Hyderabad,30000
1007,Tarun,Chennai,17000
1008,Rittik,Durgapur,45000
1009,Barun,Hyderabad,39000
1010,Utpal,Lucknow,20000

</pre>

<hr>

Search on Google with the search string "SQLite Manager online".<br>
And click on the URL - https://extendsclass.com/sqlite-browser.html

<hr>
