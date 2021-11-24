---
content_type: page
parent_title: In-Class Activities
parent_uid: 09700340-607a-547c-da2b-20b3c55a84bd
title: Efficiency
uid: 436a6df8-716e-9aca-1593-7503a10e439d
---

The purpose of this activity is to learn more about predicting efficiency using engineering models, specifically the keystroke-level model discussed in class.

Suppose we're designing a form for entering an address, and we're trying to decide between the two alternative interfaces for entering a US state shown below. The interface on the left is a drop-down menu with a list of states to choose from, and the interface on the right is a text field for entering the state's 2-letter abbreviation (e.g. MA for Massachusetts).

| State: select a state Alabama Arizona Arkansas California Colorado Connecticut Delaware District of Columbia Florida Georgia Idaho Illinois Indiana Iowa Kansas Kentucky Louisiana Maine Maryland Massachusetts Michigan Minnesota Mississippi Missouri Montana Nebraska Nevada New Hampshire New Jersey New Mexico New York North Carolina North Dakota Ohio Oklahoma Oregon Pennsylvania Rhode Island South Carolina South Dakota Tennessee Texas Utah Vermont Virginia Washington West Virginia Wisconsin Wyoming | State:  

Use the keystroke-level model to model the process of choosing Massachusetts using each of the following methods. Assume that the keyboard focus is already on the State field, and the user's hands are already on the device they need. Start by writing down the actions required; then assign K, B, P, H, and M labels to each action; and finally estimate the total time using the **KLM calculator** found below.

> _Method A:_ Using the mouse to pick Massachusetts from the drop-down menu. (Use the simplest form of the Pointing operator to estimate the times.)
> 
> _Method B:_ Using the keyboard to pick Massachusetts from the drop-down menu. (There are several ways to do this; pick one.)
> 
> _Method C:_ Using the keyboard to type MA into the text box.

Keystroke Level Model (KLM) Calculator
--------------------------------------

function recalculate() { var time = klm(get("actions").value) get("time").innerHTML = time } function klm(str) { var t = count(str, "K") \* get("K").value + count(str, "B") \* get("B").value + count(str, "P") \* get("P").value + count(str, "H") \* get("H").value + count(str, "M") \* get("M").value return t.toFixed(2) } function count(str, letter) { var matches = str.match(new RegExp(letter,"gi")) return matches ? matches.length : 0 } function get(id) { return document.getElementById(id) }

Enter an action string below to calculate its cost in the Keystroke Level Model.

| Actions:  || {{< td-colspan 2 >}}{{< /td-colspan >}} ||
| Time:  || {{< td-colspan 2 >}}5.50 sec{{< /td-colspan >}} || {{< br >}}{{< br >}} | &nbsp; | **K**eystroke |  sec |
| &nbsp; | **B**utton |  sec |
| &nbsp; | **P**oint |  sec |
| &nbsp; | **H**ome |  sec |
| &nbsp; | **M**ental |  sec 

### References

*   Card, Moran, & Newell, "[The keystroke-level model for user performance time with interactive systems](http://doi.acm.org/10.1145/358886.358895)," _CACM_, July 1980.
*   Card, Moran, & Newell, _The Psychology of Human-Computer Interaction_, CRC, 1986.
*   Kieras, David, "![This resource may not render correctly in a screen reader.](/images/inacessible.gif)[Using the Keystroke-Level Model to Estimate Execution Times, (PDF)](http://www.cs.loyola.edu/~lawrie/CS774/S06/homework/klm.pdf)" 2001.