UML State Machine Diagram
=========================

The state machine diagram is also called the Statechart or State Transition diagram, which shows the order of states underwent by an object within the system. It captures the software system's behavior. It models the behavior of a class, a subsystem, a package, and a complete system.

It tends out to be an efficient way of modeling the interactions and collaborations in the external entities and the system. It models event-based systems to handle the state of an object. It also defines several distinct states of a component within the system. Each object/component has a specific state.

Following are the types of a state machine diagram that are given below:

1.  **Behavioral state machine**  
    The behavioral state machine diagram records the behavior of an object within the system. It depicts an implementation of a particular entity. It models the behavior of the system.
2.  **Protocol state machine**  
    It captures the behavior of the protocol. The protocol state machine depicts the change in the state of the protocol and parallel changes within the system. But it does not portray the implementation of a particular component.

Why State Machine Diagram?
--------------------------

Since it records the dynamic view of a system, it portrays the behavior of a software application. During a lifespan, an object underwent several states, such that the lifespan exist until the program is executing. Each state depicts some useful information about the object.

It blueprints an interactive system that response back to either the internal events or the external ones. The execution flow from one state to another is represented by a state machine diagram. It visualizes an object state from its creation to its termination.

The main purpose is to depict each state of an individual object. It represents an interactive system and the entities inside the system. It records the dynamic behavior of the system.

Notation of a State Machine Diagram
-----------------------------------

Following are the notations of a state machine diagram enlisted below:

![UML State Machine Diagram](https://static.javatpoint.com/tutorial/uml/images/uml-state-machine-diagram.png)

1.  **Initial state:** It defines the initial state (beginning) of a system, and it is represented by a black filled circle.
2.  **Final state:** It represents the final state (end) of a system. It is denoted by a filled circle present within a circle.
3.  **Decision box:** It is of diamond shape that represents the decisions to be made on the basis of an evaluated guard.
4.  **Transition:** A change of control from one state to another due to the occurrence of some event is termed as a transition. It is represented by an arrow labeled with an event due to which the change has ensued.
5.  **State box:** It depicts the conditions or circumstances of a particular object of a class at a specific point of time. A rectangle with round corners is used to represent the state box.

Types of State
--------------

The UML consist of three states:

1.  **Simple state:** It does not constitute any substructure.
2.  **Composite state:** It consists of nested states (substates), such that it does not contain more than one initial state and one final state. It can be nested to any level.
3.  **Submachine state:** The submachine state is semantically identical to the composite state, but it can be reused.

How to Draw a State Machine Diagram?
------------------------------------

The state machine diagram is used to portray various states underwent by an object. The change in one state to another is due to the occurrence of some event. All of the possible states of a particular component must be identified before drawing a state machine diagram.

The primary focus of the state machine diagram is to depict the states of a system. These states are essential while drawing a state transition diagram. The objects, states, and events due to which the state transition occurs must be acknowledged before the implementation of a state machine diagram.

Following are the steps that are to be incorporated while drawing a state machine diagram:

1.  A unique and understandable name should be assigned to the state transition that describes the behavior of the system.
2.  Out of multiple objects, only the essential objects are implemented.
3.  A proper name should be given to the events and the transitions.

When to use a State Machine Diagram?
------------------------------------

The state machine diagram implements the real-world models as well as the object-oriented systems. It records the dynamic behavior of the system, which is used to differentiate between the dynamic and static behavior of a system.

It portrays the changes underwent by an object from the start to the end. It basically envisions how triggering an event can cause a change within the system.

State machine diagram is used for:

1.  For modeling the object states of a system.
2.  For modeling the reactive system as it consists of reactive objects.
3.  For pinpointing the events responsible for state transitions.
4.  For implementing forward and reverse engineering.

Example of a State Machine Diagram
----------------------------------

An example of a top-level state machine diagram showing Bank Automated Teller Machine (ATM) is given below.

Initially, the ATM is turned off. After the power supply is turned on, the ATM starts performing the startup action and enters into the **Self Test** state. If the test fails, the ATM will enter into the **Out Of** **Service** state, or it will undergo **a triggerless transition** to the **Idle** state. This is the state where the customer waits for the interaction. 

Whenever the customer inserts the bank or credit card in the ATM's card reader, the ATM state changes from **Idle** to **Serving Customer**, the entry action **readCard** is performed after entering into **Serving Customer** state. Since the customer can cancel the transaction at any instant, so the transition from **Serving Customer** state back to the **Idle** state could be triggered by **cancel** event.

![UML State Machine Diagram](https://static.javatpoint.com/tutorial/uml/images/uml-state-machine-diagram2.png)

Here the **Serving Customer** is a composite state with sequential substates that are **Customer Authentication, Selecting Transaction,** and **Transaction**.

**Customer Authentication** and **Transaction** are the composite states itself is displayed by a hidden decomposition indication icon. After the transaction is finished, the **Serving Customer** encompasses a triggerless transition back to the **Idle** state. On leaving the state, it undergoes the exit action **ejectCard** that discharges the customer card.

State Machine vs. Flowchart
---------------------------

State Machine

Flowchart

It portrays several states of a system.

It demonstrates the execution flow of a program.

It encompasses the concept of WAIT, i.e., wait for an event or an action.

It does not constitute the concept of WAIT.

It is for real-world modeling systems.

It envisions the branching sequence of a system.

It is a modeling diagram.

It is a data flow diagram (DFD)

It is concerned with several states of a system.

It focuses on control flow and path.