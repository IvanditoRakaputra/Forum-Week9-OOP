# Forum-Week9-OOP

### Ivandito Rakaputra - 2602119303

A large company with locations in different cities has taken an OOP approach in creating an administration program that manages all aspects of its business. These aspects include:

- the sale of all the different products that the company manages

- the salaries for managers, office staff and sales personnel.

### 1.(a) By making use of an example from the above scenario, distinguish between a class and an instantiation of a class. (3 points)

- Class is can also be defines the common properties and behaviors of a certain type of object. Class describes the characteristics and actions that objects of that specific class can have. Instantiation, known as an object, is a specific instance of a class. It is created based on the blueprint provided by the class which follow the behaviour. 

The different modules in the program each open a graphical user interface (GUI). Each GUI has a similar design but contains differences specific to each module.

### (b) By giving two examples, explain how the principles of inheritance can be incorporated into the design of this administration program. (4 points)
- The inheritance basically allows to create new classes based on existing classes. For example, from 'Product' superclass, we can get Cloth, Beverages,etc, as the subclass. Another example, the subclass employee, staff, etc, Inherits the properties and behaviors of the superclass 'Jobs', and it can also have its own specific methods and properties.

### (c) Describe how the use of libraries can facilitate the development of programs like this company’s administration program. (3 points)
- The use of libraries is that we can import its classes and use their methods, objects, and functionalities. Libraries also help us to reduce development time, and allowing developers to focus on more higher-level algorithm rather than low-level implementation details.

### 2. The company employs several sales personnel to sell its products to different retailers. Each branch of the company keeps track of its own sales with a suite of programs that include the two classes SalesPerson and Sales.

```

public class SalesPerson {

// each object contains details of one salesperson

private String id;

private Sales[] salesHistory; // details of the different sales

private int count = 0; // number of sales made



//constructor for a new salesperson

public SalesPerson(String id){

// code missing

}

 

// constructor for a salesperson transferred (together with their sales details) from another branch

public SalesPerson(String id, Sales[] s, int c){

// code missing

}

 

public int getCount(){return count;}

public String getId() {return id;}

public void setSalesHistory(Sales s){

salesHistory[count] = s;

count = count +1;

}

 

public double calcTotalSales(){

// calculates total sales for the salesperson

// code missing

}

 

public Sales largestSale(){

// calculates the sale with the largest value

// code missing

}

}

```

Each instance variable is initialized when a SalesPerson object is instantiated.

### (a) Complete the constructor public SalesPerson(String id), from the SalesPerson class. (2 points)

```

... 

 public SalesPerson(String id) {
	this.id = id;
	this.salesHistory = new Sales[100];
    }
    
...

```

### (b) Explain why accessor methods are necessary for the SalesPerson class. (3 points)

```

public class Sales {

    // each object contains details of one sale

    private String itemId;     // id of the item

    private double value;      // the price of one item

    private int quantity;      // the number of the items sold

    // constructor missing

    public double getValue() {return value;}

    public int getQuantity() {return quantity;}

}

```

- Accessor methods or getter setter is necessary because it provide controlled access to the private fields (variables) of a class. 

### (c) (i) Construct unified modelling language (UML) diagrams to clearly show the relationship between the SalesPerson and Sales classes.

Note: There is no need to include mutator or accessor methods or a constructor. (4 points)

![img](file:///C:/Users/Ivandito/Downloads/UML%20Diagram%20%232.png)
