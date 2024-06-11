## Mediator Pattern

This repository contains a simple and clear implementation of the Mediator Design Pattern in C#. 

The Mediator Pattern is a behavioral design pattern that allows you to reduce chaotic dependencies between objects. Instead, they communicate indirectly through a mediator object.

The Mediator Pattern is used to define an object that encapsulates how a set of objects interact. This pattern promotes loose coupling by keeping objects from referring to each other explicitly, and it allows their interaction to be varied independently.

##  Features
Encapsulates object interaction logic in a single place.
Promotes loose coupling between objects.
Enhances code maintainability and scalability.

// Create instances of colleagues and mediator
ConcreteMediator mediator = new ConcreteMediator();

ConcreteColleague1 colleague1 = new ConcreteColleague1(mediator);

ConcreteColleague2 colleague2 = new ConcreteColleague2(mediator);

// Register colleagues with the mediator

mediator.Colleague1 = colleague1;

mediator.Colleague2 = colleague2;

// Colleagues interact indirectly through the mediator

colleague1.Send("Message from Colleague 1");

colleague2.Send("Message from Colleague 2");
