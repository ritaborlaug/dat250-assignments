
Link to my code for experiment 2: https://github.com/ritaborlaug/dat250-jpa-tutorial 

The database that is used is h2. This can be seen in the persistence.xml -file and in the pom.xml -file where the h2 database is listed as a dependency. 
The files are stored in a filed called DB.mv.db, located inside the jpa-tutorial project folder. 
It runs when the project is run, and Hibernate automatically creates the tables. Because it is written DB_CLOSE_DELAY=-1 in the persistence file, the database will still persist after the connections are closed. 

To inspect the database tables that was created, I downloaded the h2 database engine. This created a file called h2-2.2.222.jar that I added to the project folder. This made it possible to use the h2 console and visually see the tables. I have added screenshots of the database tables as png files. 
I first thought that five tables would be made since we implemented five classes, but after having attended the lectures on object-relational-mapping, I understood that it would be made more than five tables. 

When I first startet to implement the classes, I struggled to make the tests pass.After a while I found out that I had made my own variable names in some of the classes that did not match the test-cases. This led to some trouble with the set- and get-methods. I therefore decided to use lombok to create automatic setters and getters to make things easier.


