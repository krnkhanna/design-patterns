_This is my summary of the Design Patterns. I use it while learning and as quick reference._

# Design Patterns

## 1. TABLE OF CONTENTS

- [1. TABLE OF CONTENTS](#1.-table-of-contents)
- [2. SOLID PRINCIPLES](#2.-solid-principles)
  - [2.1. SINGLE RESPONSIBILITY PRINCIPLES](#2.1.-single-responsibility-principle)
  - [2.2. OPEN CLOSED PRINCIPLES](#2.2.-open-closed-principle)
  - [2.3. LISKOV'S SUBSTITUTION PRINCIPLES](#2.3.-liskov's-substitution-principle)
  - [2.4. INTERFACE SEGREGATION PRINCIPLES](#2.4.-interface-segregation-principle)
  - [2.5. DEPENDENCY INVERSION PRINCIPLES](#2.5.-dependency-inversion-principle)
- [3. CREATIONAL PATTERNS](#3.-creational-patterns)
  - [3.1. SINGLETON DESIGN PATTERN](#3.1.-singleton-design-pattern)
  - [3.2. FACTORY DESIGN PATTERN](#3.2.-factory-design-pattern)
  - [3.3. FACTORY METHOD DESIGN PATTERN](#3.3.-factory-method-design-pattern)
  - [3.4. ABSTRACT FACTORY DESIGN PATTERN](#3.4.-abstract-factory-design-pattern)
  - [3.5. BUILDER DESIGN PATTERN](#3.5.-builder-design-pattern)
  - [3.6. PROTOTYPE DESIGN PATTERN](#3.6.-prototype-design-pattern)
- [4. BEHAVIOURAL PATTERNS](#4.-behavioural-patterns-design-pattern)
  - [4.1. CHAIN OF RESPONSIBILITY DESIGN PATTERN](#4.1.-chain-of-responsibility-design-pattern)
  - [4.2. COMMAND DESIGN PATTERN](#4.2.-command-design-pattern)
  - [4.3. ITERATOR DESIGN PATTERN](#4.3.-iterator-design-pattern)
  - [4.4. MEDIATOR DESIGN PATTERN](#4.4.-mediator-design-pattern)
  - [4.5. MOMENTO DESIGN PATTERN](#4.5.-momento-design-pattern)
  - [4.6. OBSERVER DESIGN PATTERN](#4.6.-observer-design-pattern)
  - [4.7. STRATEGY DESIGN PATTERN](#4.7.-strategy-design-pattern)
  - [4.8. TEMPLATE DESIGN PATTERN](#4.8.-template-design-pattern)
  - [4.9. VISITOR DESIGN PATTERN](#4.9.-visitor-design-pattern)
  - [4.10. NULL OBJECT DESIGN PATTERN](#4.10.-null-object-design-pattern)
- [5. STRUCTURAL PATTERNS](#5.-structural-patterns)
  - [5.1. ADAPTER DESIGN PATTERN](#5.1.-adapter-design-pattern)
  - [5.2. BRIDGE DESIGN PATTERN](#5.2.-bridge-design-pattern)
  - [5.3. COMPOSITE DESIGN PATTERN](#5.3.-composite-design-pattern)
  - [5.4. DECORATOR DESIGN PATTERN](#5.4.-decorator-design-pattern)
  - [5.5. FLY WEIGHT DESIGN PATTERN](#5.5.-fly-weight-design-pattern)
  - [5.6. PROXY DESIGN PATTERN](#5.6.-proxy-design-pattern)

## 2. SOLID PRINCIPLES

### 2.1. SINGLE RESPONSIBILITY PRINCIPLE

A class should have only one reason to change. This principle states that if we have 2 reasons to change for a class, we have to split the functionality in 2 classes. Each class will handle only 1 responsibility.

Example: Email Sending: 1 responsibility of sending email with pop3 or Imap and another responsibility is changing content.

### 2.2. OPEN CLOSED PRINCIPLE

Software entities like classes, modules and functions should be open for extension but closed for modifications. The design should be done in a way to allow the adding of new functionality as new classes keeping existing code unchanged as much as possible. There are design patterns like `Decorator Design Pattern` that help us extend code without changing it.

### 2.3. LISKOV'S SUBSTITUTION PRINCIPLE

Derived types must be completely substitutable for their base types. We must make sure that the new derived classes just extend without replacing the functionality of the base class. If a program module is using a base class then the reference to the base class can be replaced with a derived class without affecting the functionality of a program module. This principle is just an extension of the open close principle.

### 2.4. INTERFACE SEGREGATION PRINCIPLE

Clients should not be forced to implement interfaces they don't use. If the client is forced to implement the full interface and to write some dummy methods such an interface is named fat interface or polluted interface. Having an interface pollution is not a good solution and might induce inappropriate behaviour in the system. Instead of one fat interface many small interfaces are prefered.

### 2.5. DEPENDENCY INVERSION PRINCIPLE

High level modules should not depend on low level modules but should depend on abstractions and absractions should not depend on details but details should depend on abstractions. Design patterns like `Factory Design Pattern` , `Abstract Factory Design Pattern` etc. can be used to implement dependency inversion and `Template Design Pattern` is an example where the dependency inversion principle is applied.

## 3. CREATIONAL PATTERNS

Abstract the instantiation process.

### 3.1. SINGLETON DESIGN PATTERN

Singleton Design Pattern ensures only one instance of a class is created and provide a global access point to the object.

### 3.2. FACTORY DESIGN PATTERN

Factoy Design Pattern is used to create objects without exposing the instantiation logic to the client and refers to the newly created object through a common interface.

### 3.3. FACTORY METHOD DESIGN PATTERN

### 3.4. ABSTRACT FACTORY DESIGN PATTERN

### 3.5. BUILDER DESIGN PATTERN

Builder Design Pattern provides a mechanism for building complex object that is indepenedent from the ones that makes the object. This pattern allows a client to construct a complex object by specifying only its type and content being shielded from the details. This was the construction process can be used to create different representations.

Builder Design Pattern is used when:

1. The creation algorithm of a complex object is independent from the parts that actually compose the object.

### 3.6. PROTOTYPE DESIGN PATTERN

If the cost of creating a new object is large and creation is resource intensive we can clone the object.
Prototype Design Pattern allows an object ti create customized objects without knowing their class or any details of how to create them.

### 3.7. OBJECT POOL DESIGN PATTERN

Object Pool Design Pattern offers a mechanism to reuse objects that are expensive to create.

## 4. BEHAVIOURAL PATTERNS DESIGN PATTERN

### 4.1. CHAIN OF RESPONSIBILITY DESIGN PATTERN

### 4.2. COMMAND DESIGN PATTERN

The intent of Command Design Pattern is to encapsulate a request in an object.

### 4.3. ITERATOR DESIGN PATTERN

### 4.4. MEDIATOR DESIGN PATTERN

### 4.5. MOMENTO DESIGN PATTERN

### 4.6. OBSERVER DESIGN PATTERN

### 4.7. STRATEGY DESIGN PATTERN

The intent of Strategy Design Pattern is to define a family of algorithms and let

### 4.8. TEMPLATE DESIGN PATTERN

Define the skeleton of an algorithm in an operation defering some steps to the subclasses. A template method defines an algorithm in a base class using abstract operations that subclasses override to provide concrete behaviour.
Strategy Design Pattern is similar to Template Design Pattern, the difference consists in the fact that strategy uses a delegation while the template method uses inheritance.
Template Design Pattern uses an inverted control structure. This refers to the fact that instead of calling the methods of base class from the subclasses, the methods of subclass are called in the template method from superclass.

### 4.9. VISITOR DESIGN PATTERN

### 4.10. NULL OBJECT DESIGN PATTERN

## 5. STRUCTURAL PATTERNS

### 5.1. ADAPTER DESIGN PATTERN

Adapter Design Pattern lets classes work together that could not otherwise because of incompatible interfaces. It helps convert the interface of a class into another interfaces that clients expect.
Like adapter in real world it is used to be an interface a bridge between two objects.
It can be used when you have an object offering the same feature but exposing a different interface.

### 5.2. BRIDGE DESIGN PATTERN

The intent of Bridge Design Pattern is to decouple abstraction from implementation so that

### 5.3. COMPOSITE DESIGN PATTERN

### 5.4. DECORATOR DESIGN PATTERN

The intent of this pattern is to ass additional responsibilities dynamically to an object. Extending an object's functionality can be done at compile time by using inheritance however it might be necessary to extend an object's functionality dynamically as an object is needed. It can also be used when subclassing would be impossible due to a large number of subclasses that could result.

### 5.5. FLY WEIGHT DESIGN PATTERN

The intent of this pattern is to use sharing to support a large number of objects that have part of their internal state in common where as the other part of the state can vary. To be used when application requires a large number of objects that have some shared state among them.
Example: A game of war, where there is a large number of soldier objects. A soldier object maintains the graphical representation of a soldier, soldier behaviour such as motion and weapons in addition to health and location on the war terrain. Creating large number of soldier objects is necessary however it would incur a huge cost.

### 5.6. PROXY DESIGN PATTERN

The intent of Proxy Design Pattern is to provide a placeholder for an object to control reference to it. The ability to control the access to an object can be required for a variety of reasons:

1. Controlling when a costly object needs to be instantiated and initialized.
2. Giving different access rights to an object.
