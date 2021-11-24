---
content_type: page
parent_title: In-Class Activities
parent_uid: 09700340-607a-547c-da2b-20b3c55a84bd
title: UI Software Architecture
uid: b101ce27-19e1-b207-31ff-35904236fdbb
---

![A screen capture of a simple HTML form, consisting of a single text entry field, a submit button, and a logout link.](BASEURL_PLACEHOLDER/resources/ac9-1)  
© Source unknown. All rights reserved.  
This content is excluded from our Creative  
Commons license. For more information,  
see [http://ocw.mit.edu/fairuse](/fairuse).

The goal of this activity is to explore some of the main structuring patterns of GUI software: the view tree, listeners, and model-view-controller. We'll do it using HTML, Javascript, and jQuery, along with a handy online HTML editor:

*   [SquareFree's HTMLEdit](http://htmledit.squarefree.com/)

You'll also need a modern standards-compliant web browser with developer tools installed in it. We recommend either:

*   [Google Chrome](http://www.google.com/chrome) (which has developer tools baked in, at View >> Developer >> Developer Tools)
*   [Mozilla Firefox](http://getfirefox.com) (which needs [Firebug](http://getfirebug.com) installed to be useful for development)

Make and Inspect a View Tree
----------------------------

Use the editor to construct the simple HTML user interface you see on the right. You'll need to use HTML elements like div, textarea, button, and a. Wrap the whole thing in a div element.

Use the developer tools in your browser to display the HTML tree and find the textarea node you just created.

Attach a Listener
-----------------

Add jQuery to your web page, which you can do with the following line of code:

<script src="http://code.jquery.com/jquery-1.5.min.js"></script>

Attach an event listener to your Send button that calls console.log() to display the text area's contents in your developer console. You will find it useful to:

*   put [id attributes](http://www.w3.org/TR/html401/struct/global.html#h-7.5.2) on your HTML elements
*   use the selector [$("#id")](http://api.jquery.com/id-selector/) to find an element with a particular id
*   use the jQuery [.click()](http://api.jquery.com/click/) method to attach an event handler. (There are also ways to declaratively attach an event handler in the HTML code, such as the onclick attribute, but it's generally better to do it procedurally.)
*   use the jQuery [.val()](http://api.jquery.com/val/) method to get the value of a textarea

Modify the View Tree
--------------------

Now we want to display a log of sent messages in the UI itself. First add the following HTML code to the end of your UI, so that you have a place to put the messages:

<div id="sent" style="font-style: italic">
    <div>Sent messages appear here.</div>
</div>

Enhance your event listener on the Send button so that it appends the textarea's contents to this list. For example, if the textarea has "message 1" in it, then pressing Send should change the page as follows:

<div id="sent" style="font-style: italic">
    <div>Sent messages appear here.</div>
    <div>message 1</div>
</div>

There are several ways to do this. You may find the following jQuery methods useful:

*   the [.html()](http://api.jquery.com/html/) method to get or set the subtree under a node
*   the [.text()](http://api.jquery.com/text/) method to get or set the text inside a node
*   the [.append()](http://api.jquery.com/append/) method to add children to a node
*   the [$("html")](http://api.jquery.com/jQuery/#jQuery2) function to create a subtree of HTML