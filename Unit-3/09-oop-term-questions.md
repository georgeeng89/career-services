# Terms

## Object Oriented Terms

What are the 3 tenets of object-oriented programming?
> Encapsulation, Inheritance and Polymorphism

(alternatively) What are the 4 tenets of object-oriented programming?
> Abstraction, Encapsulation, Inheritance and Polymorphism

What are classes and objects (and the difference between the two)?
> A class is a blueprint for an object.  Class definitions define the types of state and behavior an instance can have.  Objects are instances of classes.  They actually hold the state.

What is a constructor?
> A constructor is a special method that gets called automatically when an object is instantiated.  Constructors are where you setup the initial state of the object, often times based on the arguments passed to the object when instantiating it.

What is instantiation?
> Creating a new instance of a class.  Typically done with a `new` keyword or method such as `new Person()` or (Ruby) `Person.new`

What is a method (as opposed to, say, a C function)?
> A method is a function that is bound to an object.  Methods have access to a `this` that refers to that instance.

What is inheritance?
> Inheritance allows developers to create classes that share behavior with other classes without having to duplicate the parent classes methods.  Subclasses can define new state, add behaviors or refine behaviors from parent classes.

What is encapsulation?
> Encapsulation is the practice of hiding data such that code outside of the class cannot directly mutate internal state.  Also known as data hiding, encapsulation allows developers to change the behavior of a class without changing the public interface, therefor making code easier to refactor.

What is polymorphism (without resorting to _just_ examples)?
> Polymorphism means a few things, but generally it's the pattern in OOP where different classes can implement the same method signatures, but have different implementations.  For example if you had a `CSVImporter` class that had an `doImport` method, and you had a `JSONImporter` class that had a `doImport` method.  Each class shares the same interface for `doImport`, other methods can work with instances of either class.

What does abstraction mean in the broad OOP sense?
> Abstraction refers to the act of modeling things or processes in code.  For example modeling a customer with a `Customer` class, or modeling an order with classes such as `Order` and `OrderItem`.

What is a mutator (aka "setter" or "command method")?
> A mutator is a method that changes the state of an object.

What is an accessor (aka "getter" or "query method")?
> An accessor is a method that does _not_ change state, but instead returns a value, typically related to the state of an object.  Getters and setters (accessors and mutators / command methods and query methods) are the primary way in which to achieve Encapsulation.

What is a static method (aka "class method")?
> A method that can be called directly on a class, rather than any particular instance of that class.  For example `Person.calculateAge(birthdate)` as opposed to `person.age()`

What is a superclass (aka "parent class" or "base class")?
> Classes can inherit from other classes.  When a class inherits from another class, the class being inherited from is called the superclass.

What is a subclass (aka "child class" or "derived class")?
> When one class inherits from another, the class that is _inheriting_ is called the subclass.
What is composition/aggregation?
> Composition refers to having instance variables that are instances of other classes.  If you are building an ETL (extract, transform and load) you might have an `ETL` class that is "composed of" an `Extractor`, a `Transformer` and a `Loader`, where "composed of" means having properties such as `extractor`, `transformer` and `loader`.

What is delegation/forwarding?
> Delegation and forwarding refer to the concept of an instance receiving a message (having a method called in) and doing nothing other than calling a method on a composed object.

What is an abstract class?
> An abstract class is a class that cannot be directly instantiated, but that has methods that can be inherited.

What is an interface/protocol (and different from abstract class)?
> Generally speaking interfaces do not have any implementation, they are just method signatures.

What is method overriding?
> Overriding a method refers to the concept that a subclass can implement a method with the same method signature as the superclass.

What is method overloading (and difference from overriding)?
> Method overloading refers to when there are two different method signatures that share the same name.  For example you might have an `htmlTag(content)` signature, an `htmlTag(content, attributes)` signature and an `htmlTag(content, attributes, selfClosing)` method signature.  These are three different signatures - two of which override the first.

What are "is-a" versus "has-a" relationships (with examples)?
> Is-a relationships are inheritance relationships - it means that an instance "is" of a certain type.  "has-a" relationships are composition relationships - it means that an instance has a reference to an instance of another type.  So if you have a `Dancer` and `BreakDancer` class, you would say that `BreakDancer` "is a" `Dancer`.  If you had a `Browser` class and a `BackButton` class, you would say that the `Browser` class "has a" `BackButton`.

What are method signatures (what's included in one)?
> Method signatures are comprised of the name of the method, the number of arguments and the types of those arguments.

What is method visibility (e.g. public/private/other)?
> Classes can define how certain properties and method can be used from subclasses or code outside of the class.  Private methods may only be called by instances of that class.  Protected methods can be called by instances of the class and any subclass.  Public methods may be called by any code that can access the class.

What does it mean to compose an object?
> Composition is when objects are assembled out of smaller pieces, rather than inherited and specialized.

What is an interface?
> A set of methods that an object is guaranteed to have.

What's the difference between a method and a function?
> A method belongs to an object.

What is a virtual method (aka pure virtual method)?
> An empty method on an abstract superclass.
