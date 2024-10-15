Prompt: What is a class in C#?

Response:
In C#, a class is a blueprint or template for creating objects. It defines the properties (attributes or data) and methods (actions or behaviors) that the objects created from the class will have. A class is like a design for a house, while an object is the actual house built using that design.
Key Concepts of a Class in C#:

Class Definition: It defines the structure of an object, specifying what data (fields or properties) and behaviors (methods or functions) the object will have.
class Car
{
    // Fields or properties (attributes)
    public string brand;
    public string model;
    public int year;

    // Methods (actions/behaviors)
    public void Start()
    {
        Console.WriteLine("Car is starting...");
    }
}

Object: An instance of a class. You create objects from a class using the new keyword.

Car myCar = new Car(); // 'myCar' is an object of class 'Car'
Properties: Variables that hold data inside the class. In the example, brand, model, and year are properties of the Car class.
myCar.brand = "Toyota";
myCar.model = "Corolla";
myCar.year = 2020;

Methods: Functions that define the actions the object can perform. In the Car class, the Start method describes what happens when the car starts.

myCar.Start(); // Calls the Start method for the 'myCar' object

Constructor: A special method that gets called when an object is created. It allows you to initialize properties when the object is instantiated.

class Car
{
    public string brand;
    public string model;
    public int year;

    // Constructor
    public Car(string carBrand, string carModel, int carYear)
    {
        brand = carBrand;
        model = carModel;
        year = carYear;
    }

    public void Start()
    {
        Console.WriteLine($"{brand} {model} is starting...");
    }
}

Car myCar = new Car("Toyota", "Corolla", 2020); // Constructor initializes the properties

Encapsulation: One of the principles of Object-Oriented Programming (OOP), where the internal details of the class are hidden from outside code, and only specific methods or properties are exposed.

Access Modifiers: Control the visibility of properties and methods outside the class.

public: Can be accessed from outside the class.
private: Can only be accessed within the class itself.

Why Use Classes?
Reusability: Once a class is defined, you can create as many objects from it as needed.
Organization: Classes help in organizing code into logical units.
Encapsulation: Protects the internal workings of a class while allowing interaction through public methods or properties.
Abstraction: You can define high-level operations and hide complex details inside methods.
Inheritance: A class can inherit features from another class, which promotes code reuse.
In summary, classes are fundamental in C# for building objects and organizing code in an efficient, reusable, and maintainable way.