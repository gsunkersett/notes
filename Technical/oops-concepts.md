# OOPs concepts

#Technical

### Core OOP principles in C#

1. **Abstraction**
    - Objects: Imagine objects as real-world things like a car, a bank account, or even a window on your screen. Each object has its own unique set of properties (data) that describe its state and behaviors (methods) that define its actions.
    - Classes: A class acts as a blueprint that defines the template for creating objects. It specifies the properties (variables) that objects of that class will have and the methods (functions) that objects can perform. This allows you to create multiple objects (instances) from a single class, each with its own copy of the properties but potentially different states.

2. **Encapsulation**

    - Encapsulation is the concept of bundling data and methods together within a class. This promotes data security and reduces the risk of accidental modifications. You can control access to this data using access modifiers:
        - public: Members (properties and methods) are accessible from anywhere in your code.
        - private: Members are only accessible within the class itself, protecting them from unintended changes from outside code.
        - protected: Members are accessible within the class and by subclasses that inherit from it, allowing for controlled inheritance behavior.

3. **Inheritance**
    - Inheritance allows you to create hierarchical relationships between classes. A new class (subclass) can inherit properties and behaviors from an existing class (superclass). This promotes code reuse and simplifies development. Imagine a general Vehicle class with properties like color and speed and methods like accelerate and brake. You can create subclasses like Car and Truck that inherit these properties and methods, and potentially add their own specialized properties and methods (e.g., Car.openTrunk() or Truck.towCapacity).

4. **Polymorphism**
    - Polymorphism refers to the ability of objects to respond differently to the same message. This allows for flexible and dynamic behavior in your code. There are two main ways to achieve polymorphism:
        - Method Overloading: This involves defining multiple methods with the same name but different parameter lists within the same class. The appropriate method is called based on the arguments provided at runtime. For example, a Draw() method could take different arguments to draw a circle, rectangle, or line depending on the provided parameters.
        - Method Overriding: Subclasses can override methods inherited from their superclass. This allows you to customize the behavior of an inherited method in the subclass. For instance, a Draw() method in a Car class might draw a four-wheeled vehicle, while a Draw() method in a Truck class might draw a vehicle with six wheels.

By effectively using these OOP concepts, you can structure your C# code in a way that's modular, maintainable, reusable, and promotes better code organization and easier collaboration.
