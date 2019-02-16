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
- [3.1. SINGLETON](#3.1.-singleton)
- [3.2. FACTORY](#3.2.-factory)
- [3.3. FACTORY METHOD](#3.3.-factory-method)
- [3.4. ABSTRACT FACTORY](#3.4.-abstract-factory)
- [3.5. BUILDER](#3.5.-builder)
- [3.6. PROTOTYPE](#3.6.-prototype)
- [4. BEHAVIOURAL PATTERNS](#4.-behavioural-patterns)
- [4.1. CHAIN OF RESPONSIBILITY](#4.1.-chain-of-responsibility)
- [4.2. COMMAND](#4.2.-command)
- [4.3. ITERATOR](#4.3.-iterator)
- [4.4. MEDIATOR](#4.4.-mediator)
- [4.5. MOMENTO](#4.5.-momento)
- [4.6. OBSERVER](#4.6.-observer)
- [4.7. STRATEGY](#4.7.-strategy)
- [4.8. TEMPLATE](#4.8.-template)
- [4.9. VISITOR](#4.9.-visitor)
- [4.10. NULL OBJECT](#4.10.-null-object)
- [5. STRUCTURAL PATTERNS](#5.-structural-patterns)
- [5.1. ADAPTER](#5.1.-adapter)
- [5.2. BRIDGE](#5.2.-bridge)
- [5.3. COMPOSITE](#5.3.-composite)
- [5.4. DECORATOR](#5.4.-decorator)
- [5.5. FLY WEIGHT](#5.5.-fly-weight)
- [5.6. PROXY](#5.6.-proxy)

## 2. SOLID PRINCIPLES

### 2.1. SINGLE RESPONSIBILITY PRINCIPLE

A class should have only one reason to change. This principle states that if we have 2 reasons to change for a class, we have to split the functionality in 2 classes. Each class will handle only 1 responsibility.

Example: Email Sending: 1 responsibility of sending email with pop3 or Imap and another responsibility is changing content.

### 2.2. OPEN CLOSED PRINCIPLE

Software entities like classes, modules and functions should be open for extension but closed for modifications. The design should be done in a way to allow the adding of new functionality as new classes keeping existing code unchanged as much as possible. There are design patterns like Decorator pattern that help us extend code without changing it.

### 2.3. LISKOV'S SUBSTITUTION PRINCIPLE

Derived types must be completely substitutable for their base types. We must make sure that the new derived classes just extend without replacing the functionality of the base class. If a program module is using a base class then the reference to the base class can be replaced with a derived class without affecting the functionality of a program module. This principle is just an extension of the open close principle.

### 2.4. INTERFACE SEGREGATION PRINCIPLE

Clients should not be forced to implement interfaces they don't use. If the client is forced to implement the full interface and to write some dummy methods such an interface is named fat interface or polluted interface. Having an interface pollution is not a good solution and might induce inappropriate behaviour in the system. Instead of one fat interface many small interfaces are prefered.

### 2.5. DEPENDENCY INVERSION PRINCIPLE

## 3. CREATIONAL PATTERNS

### 3.1. SINGLETON

### 3.2. FACTORY

### 3.3. FACTORY METHOD

### 3.4. ABSTRACT FACTORY

### 3.5. BUILDER

### 3.6. PROTOTYPE

### 3.7. OBJECT POOL

## 4. BEHAVIOURAL PATTERNS

### 4.1. CHAIN OF RESPONSIBILITY

### 4.2. COMMAND

### 4.3. ITERATOR

### 4.4. MEDIATOR

### 4.5. MOMENTO

### 4.6. OBSERVER

### 4.7. STRATEGY

### 4.8. TEMPLATE

### 4.9. VISITOR

### 4.10. NULL OBJECT

## 5. STRUCTURAL PATTERNS

### 5.1. ADAPTER

### 5.2. BRIDGE

### 5.3. COMPOSITE

### 5.4. DECORATOR

### 5.5. FLY WEIGHT

### 5.6. PROXY
