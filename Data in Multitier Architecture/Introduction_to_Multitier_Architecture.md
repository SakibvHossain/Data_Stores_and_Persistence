**Multitier Architecture** is a term used to refer to a form of design that separates various functions of the application into their own layers. In this course, we’ll focus on how data in our application is defined and used across these layers.

It's more important to undertand the role persistence plays in an enterprise application than it is to know some specific config properties or the syntax for writing a SQL statement in Java.

**Learn:** How to write entity classes that can describe complex relationships between multiple java objects.

**Entities are used to negotiate between:**  
The **object** representation of data in Java.  
The **table** representation of data in a database.  

**Entity Design Overview:** There is no simple definition of what type of data can be an entity. Sometimes we need to represent data that's clearly object-oriented, such as users in our application, products we sell.    

JSON <---translate---> Entity <---translate---> Database Table

**Lesson Overview:**  
1.  Value vs Entity
2.  BasicTypes in Java and JDBC ()
3.  Identifiers (Entity uniqueness and how to define entities in a way that allows Java in the database to share an understanding of what constitutes a unique entity)
4.  Relationships (Finding relationship between objects)
5.  Inheritance (Finding relationship between objects both through composition and inheritance)
