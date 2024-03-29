# Value vs Entity  

**Entity**: Is nothing but a table  
**Value**: Is nothing but a values of the table   

```
@Entity
public class Address {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;

    @Column(name = "street")
    private String street;

    @Column(name = "hourse")
    private String house;

    @Column(name = "zip")
    private String zipCode;
}
```
Look at the code, the entity is the Address and the values are id, street, house, & zipcode.

---------------------------------------------------------------------------------------------------------

**Multilingual Application:** Suppose you're developing an application that allows users to enter their names in various languages. Some users might have names with characters from non-Latin alphabets, such as Cyrillic, Chinese, or Arabic. In this case, using @Nationalized ensures that the names are stored correctly in the database without losing any characters or encountering encoding issues.

```
@Entity
@Table(name = "user")
public class User {

    @Id
    @GeneratedValue
    private Long id;

    @Nationalized
    private String name; // User's name can contain characters from various languages
    
    // Other fields, constructors, getters, and setters
}
```
**International Product Catalog:** Imagine you're building an e-commerce platform that sells products worldwide. Each product may have a description that needs to be displayed in multiple languages. Using @Nationalized for the description field ensures that the descriptions can accommodate characters from different languages and are stored correctly in the database.

```
@Entity
@Table(name = "product")
public class Product {

    @Id
    @GeneratedValue
    private Long id;

    @Nationalized
    private String description; // Product description can contain characters from various languages
    
    // Other fields, constructors, getters, and setters
}
```
