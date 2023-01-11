## Assignment6
  Explain event bubbling and capture with an example

> Deadline: 11th Jan, 8 am



# Bubbling
Event bubbling is a method of event propagation in the HTML DOM API when an event is in an element inside another element, and both elements have registered a handle to that event. It is a process that starts with the element that triggered the event and then bubbles up to the containing elements in the hierarchy. In event bubbling, the event is first captured and handled by the innermost element and then propagated to outer elements. It happens when an element receives an event, and that event bubbles up (or you can say is transmitted or propagated) to its parent and ancestor elements in the DOM tree until it gets to the root element.This is the default behavior of events on elements unless you stop the propagation.The "Event Bubbling" behavior makes it possible for you to handle an event in a parent element instead of the actual element that received the event.
# Capturing
Event capturing is one of two ways to do event propagation in the HTML DOM. In event capturing, an event propagates from the outermost element to the target element. It is the opposite of event bubbling, where events propagate outwards from the target to the outer elements.Capturing happens before bubbling. The three phases of event propagation are: capturing, target, and bubbling.Event capturing is rarely used and, usually, events are handled on bubbling. When you use the on<event>-property or the two-argument method addEventListener(event, handler) to add event handlers, the events are only handled during the bubbling phase (the default case). However, you can still handle events during the capturing phase using the method given in the example below.