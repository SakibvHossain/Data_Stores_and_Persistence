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
