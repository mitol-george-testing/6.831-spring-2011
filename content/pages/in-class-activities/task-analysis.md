---
content_type: page
parent_title: In-Class Activities
parent_uid: 09700340-607a-547c-da2b-20b3c55a84bd
title: Task Analysis
uid: 1c9ae285-87b7-55df-3b1c-2af5c1e1536c
---

![A photo of the MIT classroom in which 6.831 was taught.](BASEURL_PLACEHOLDER/resources/ac6-1) The goal of this activity is to practice doing user, task and domain analysis by observing a real environment of people working. Without actual observation, task analysis is incomplete and biased. For this exercise, we'll observe the most conveniently available environment: our classroom.

Assume we're thinking of developing a system to deliver 6.831 as an _online_ course. We're not actually going to do any design in this exercise, but you should think about users, tasks, and entities from this point of view.

1\. User Analysis
-----------------

Who are the major user classes involved in the system? What are their important characteristics? Note that some relevant user classes might not have any representatives in the room right now.

2\. Task Analysis
-----------------

Pick an important user class **that you don't belong to**. Identify important tasks for this user class by observation. Structure your task analysis hierarchically, with tasks and subtasks.

A few things to think about:

*   Try to distinguish essential tasks (independent of the current in-person course) from concrete tasks (which exist in the current design, but maybe don't need to be there). Why is it important to think about this distinction?

3\. Domain Analysis
-------------------

Draw a domain model for the course. Include boxes for major user classes and for major information objects. Draw lines between the boxes for important relations. Finally, annotate the boxes with multiplicities (e.g., how many members of each user class?)