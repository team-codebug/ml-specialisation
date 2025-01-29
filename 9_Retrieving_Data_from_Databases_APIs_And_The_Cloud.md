# Retrieving Data from Databases, APIs, and the Cloud

## SQL Databases
Structured Query Language (SQL) represents a set of relational databases with fixed schemas. SQL databases store data in structured tables with predefined relationships between them. Different types of SQL databases function similarly but may have subtle differences in syntax.

### Examples of SQL Databases
- **Microsoft SQL Server**
- **Postgres**
- **MySQL**
- **AWS Redshift**
- **Oracle DB**
- **Db2 Family**

### Reading SQL Data in Python
To interact with SQL databases in Python, we can use various libraries such as `sqlite3`, `SQLAlchemy`, or `psycopg2` (for PostgreSQL). Below is an example using `sqlite3` and `pandas`:

```python
# SQL Data imports
import sqlite3 as sq3
import pandas as pd

# Initialize path to SQLite database
path = 'data/classic_rock.db'

# Create connection to SQL Database
con = sq3.Connection(path)

# Write SQL query
query = '''SELECT * FROM rock_songs'''

# Execute query and load data into pandas DataFrame
data = pd.read_sql(query, con)
```

### Explanation
- The `sqlite3` module creates a connection with the database.
- The SQL query is executed using the `pd.read_sql()` function, which fetches data and loads it into a pandas DataFrame.
- While `sqlite3` is used in this example, other libraries such as `pyodbc`, `SQLAlchemy`, and `psycopg2` can be used for different databases.

---

## NoSQL Databases
Not-only SQL (NoSQL) databases differ from relational databases in that they do not rely on structured schemas. Instead, they store data in flexible formats, which can improve performance and reduce technical overhead.

### Types of NoSQL Databases
- **Document Databases**: MongoDB, CouchDB
- **Key-Value Stores**: Riak, Voldemort, Redis
- **Graph Databases**: Neo4j, HyperGraph
- **Wide-Column Stores**: Cassandra, HBase

### Reading NoSQL Data in Python (MongoDB Example)
MongoDB is a popular document-based NoSQL database. Below is an example of how to retrieve data using Python:

```python
# Import MongoDB client
from pymongo import MongoClient
import pandas as pd

# Create a MongoDB connection
con = MongoClient()

# Select database (use con.list_database_names() to list available databases)
db = con.database_name

# Create a cursor object using a query
cursor = db.collection_name.find({})  # Empty query selects all documents

# Expand cursor and construct DataFrame
df = pd.DataFrame(list(cursor))
```

### Explanation
- The `pymongo` module is used to interact with MongoDB.
- A connection is established to the database.
- A query (`{}`) is executed to retrieve data from a collection.
- The query results are converted into a pandas DataFrame.
- MongoDB must be running for this to work.

---

## APIs and Cloud Data Access
Many organizations and cloud providers expose data through **Application Programming Interfaces (APIs)**. APIs provide an efficient way to fetch structured data from various sources.

### Reading Cloud Data in Python
If a dataset is hosted on the web, it can be directly read into pandas using a URL:

```python
# Define the data source URL
data_url = "https://example.com/data.csv"

# Read data into pandas DataFrame
df = pd.read_csv(data_url, header=None)
```

### Explanation
- The `data_url` variable stores the URL of the dataset.
- The `pd.read_csv()` function reads data from the given URL and converts it into a pandas DataFrame.
- Many cloud platforms (such as AWS, Google Cloud, and Azure) also provide APIs to fetch data programmatically.

---

## References
1. SQLite documentation: [https://www.sqlite.org/docs.html](https://www.sqlite.org/docs.html)
2. MongoDB documentation: [https://www.mongodb.com/docs/manual/](https://www.mongodb.com/docs/manual/)
3. Pandas documentation: [https://pandas.pydata.org/docs/](https://pandas.pydata.org/docs/)
4. SQLAlchemy documentation: [https://www.sqlalchemy.org/](https://www.sqlalchemy.org/)
5. Google Cloud APIs: [https://cloud.google.com/apis](https://cloud.google.com/apis)
6. AWS APIs: [https://aws.amazon.com/api-gateway/](https://aws.amazon.com/api-gateway/)
