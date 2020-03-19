# Get Sqlite with Python

**The dataset**

[American Community Survey data on college majors and job outcomes](https://github.com/fivethirtyeight/data/tree/master/college-majors)

* use : [recent-grads](https://github.com/fivethirtyeight/data/blob/master/college-majors/recent-grads.csv)

**The data dictionary**

|Column|Descriptions|
|---|---|
|Rank|The major's rank by median earnings|
|Major_code|The major's code or ID|
|Major|The name of the major|
|Major_category|The broader category the major belongs to|
|Total|The total number of people who studied the major|
|Sample_size|The sample size (unweighted) of graduates with full time jobs|
|Men|The number of male graduates|
|Women|The number of female graduates|
|ShareWomen|Women as a proportion of the total number of graduates (a number ranging from 0 to 1)|
|Employed|The number of employed graduates|

**Instructions**

Loaded a subset of the data into a table named recent_grads in a database. The subset contains the 2010-2012 data for recent college grads only. The database file we'll be working with is called jobs.db

**Library**
pysqlite  **if python2 
sqlite3 

SQLite restricts access to the database file when we're connected to a database, we need to close the connection when we're done working with it. Closing the connection allows other processes to access the database, which is important when you're in a production environment and working with other team members.

[Install](https://pypi.org/project/pysqlite/)

[Documentation](https://pysqlite.readthedocs.io/en/latest/sqlite3.html)

**Windows**
1. Install sqlite3
2. CMD prompt to installation directory
3. .\sqlite3
4. .open '_.db'

**sqlite3 Method , Python**



.fetchone()
.fetchmany(n)

When we call the fetchone() method, the Cursor instance will return a single result, and then increment its internal counter by 1. This means that if we call fetchone() again, the Cursor instance will actually return the second tuple in the results set (and increment by 1 again).

To return a single result (as a tuple), we use the Cursor method fetchone(). To return n results, we use the Cursor method fetchmany().