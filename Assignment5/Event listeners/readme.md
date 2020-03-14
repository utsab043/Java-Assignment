> # Types of EventListenerInterface:

> ## ActionListener:
```java
void actionPerformed(ActionEvent e)
```
> ## KeyListener:
```java
void keyPressed(KeyEvent e)
void keyReleased(KeyEvent e)
void keyTyped(KeyEvent e)
```
> ## MouseListener:
```java
void mouseClicked(MouseEvent e)
void mousePressed(MouseEvent e)
void mouseReleased(MouseEvent e)
void mouseEntered(MouseEvent e)
void mouseExited(MouseEvent e)
```
> ## MouseMotionListener:
```java
void mouseMoved(MouseEvent e)
void mouseDragged(MouseEvent e)
```
> ## TextListener:
```java
void textValueChanged(TextEvent e)
```

> ## WindowListener:
```java
public abstract void windowActivated(WindowEvent e);  
public abstract void windowClosed(WindowEvent e);  
public abstract void windowClosing(WindowEvent e);  
public abstract void windowDeactivated(WindowEvent e);  
public abstract void windowDeiconified(WindowEvent e);  
public abstract void windowIconified(WindowEvent e);  
public abstract void windowOpened(WindowEvent e);
```
> ## Java Event Listener interfaces
Event Classes | Listener Interfaces
------------  | -------------------
ActionEvent   |	ActionListener
MouseEvent    | MouseListener and MouseMotionListener
MouseWheelEvent | MouseWheelListener
KeyEvent	| KeyListener
ItemEvent	| ItemListener
TextEvent	| TextListener
AdjustmentEvent	| AdjustmentListener
WindowEvent	| WindowListener
ComponentEvent	| ComponentListener
ContainerEvent	| ContainerListener
FocusEvent	|  FocusListener