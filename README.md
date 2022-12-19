# ErrorDictionary

# issue 1: Port 5432 is already in use  
#Solution 1: To check what is running on port 5432, issue the following command on your terminal.
$ sudo lsof -i :5432
You might get a different output depending on what application is using the port. In my case, I had a different version of the PostgreSQL server running on my Mac, that was interfering with the Postgres.app. If you have the same problem, to kill all PostgreSQL processes, issue the following command.
$ sudo pkill -u postgres
