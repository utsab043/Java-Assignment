> # Event Objects:
Event Objects are created by AWT itself when different actions occur on the components being rendered.

On the basis of occurred events, the respective event objects are created. For example, when an user clicks a button, *ActionEvent* object is created and so on.

> ## Types Of Events In Java:

* __ActionEvent:__

When an user clicks a button, *ActionEvent* object is created.

* __ContainerEvent:__

When an user adds or removes an object from the interface, *ContainerEvent* object is created.

* __KeyEvent:__

When an user presses, types or releases a key, *KeyEvent* object is created.

* __WindowEvent:__ 

When a window is closed, activated or deactivated, *WindowEvent* object is created.

* __MouseEvent:__ 

When a mouse is clicked or pressed, *MouseEvent* object is created.

> ### Constructor Summary:

```java
EventObject(Object source)
//Constructs a prototypical Event.
```

> ### Methods Summary:

```java
EventObject.getSource() ;
// getSource() defines where the Event has initially occurred.

EventObject.toString() ;
// toString() defines string representation of event object.
```
