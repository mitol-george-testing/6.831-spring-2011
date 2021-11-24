---
content_type: page
parent_title: In-Class Activities
parent_uid: 09700340-607a-547c-da2b-20b3c55a84bd
title: Input
uid: e33273d8-0343-4f6e-27b9-c5d6431974c6
---

code { font-size: 1.3em; }

The purpose of this activity is to learn more about how user interfaces handle mouse and keyboard input. You'll need a modern standards-compliant web browser like Firefox, Opera, or Safari; don't use an old version of Internet Explorer. The exercises below use an in-browser Javascript environment that you'll find here (link will open in a new window or tab):

*   [Event Workbench](/ans7870/6/6.831/s11/ac12-event-handling.htm)

Event Dispatch and Propagation
------------------------------

The workbench is initially configured with an event listener listening for clicks on A. Which objects can you click on to fire this listener?

Add a click listener to object C (keeping the listener on A as well). Which listeners fire when you click on C? In what order do they fire? How about when you click on B?

Change your listener on C so that it _consumes_ the event. In standard browsers, this is done by calling `event.stopPropagation()`. Now which listeners fire when you click on C? How about when you click on B?

Finally, change your listener for A from a bubbling-phase listener to a **capturing** listener. Now which listeners fire when you click on C? In what order?

Event Translation
-----------------

Javascript's events for mouse clicking are `click`, `mousedown`, `mouseup`, and `dblclick`. Attach listeners for these events to one of the objects in the workbench to discover the sequence in which these events occur when the user double-clicks on that object. Which of these events are raw, and which are translated?

Mouse Movements
---------------

Javascript's event for mouse movement is `mousemove`. Add a mouse move listener to A, and display the mouse coordinates using `print(event.clientX + "," + event.clientY)`. What origin are these (x,y) positions using? How is this different from the coordinate system used by Java Swing's mouse events? (See MouseEvent in the [Java 1.5 API documentation](http://java.sun.com/j2se/1.5/docs/api/).)

Now slow down your mouse move listener. (The workbench defines a function `sleep(milliseconds)` for this purpose; e.g., `sleep(500)` waits for 500 milliseconds before it returns.) Does the browser coalesce mouse move events? How do you know? Does it coalesce mouse _click_ events?

Mouse Capture
-------------

Using your mousemove listener on A, determine whether the web browser provides _mouse capture_ by default: i.e., if you press the mouse button over A, does A continue receiving mouse events until the mouse button is released, regardless of where the mouse pointer is?

Try attaching the mousemove listener to the `window` object instead of A. Does mouse capture work now? Note that you have to move the mouse outside the whole window to really answer this question.

Would you be able to implement a scrollbar using just HTML and Javascript? Why or why not?