# Change Preventers

## Learning Goals

- Explain the change preventers pattern

## Introduction

Change preventers are code smells that make it harder to make changes to your
code at a later time. We should always remember that code is read and modified
many more times than it's written the first time, so long-term maintainability
must be a high priority for your code.

### Divergent Change

This code smell happens when a change to a method in a single class requires
many changes to other methods in the same class. This is usually an indication
that code in a specific method is too reliant on logic or data structures
outside that method.

### Shotgun Surgery

Shotgun Surgery is the opposite of Divergent Change in that it happens when a
single change to a class requires many changes to other classes. This is usually
an indication that too many classes are dependent on the functionality of a
single class.

### Parallel Inheritance Hierarchies

This smell happens when you realize that creating a subclass of one class forces
you to also create a subclass of another class. That usually means that the two
inheritance hierarchies are too tightly coupled together.
