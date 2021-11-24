---
content_type: page
parent_title: In-Class Activities
parent_uid: 09700340-607a-547c-da2b-20b3c55a84bd
title: User-centered Design
uid: 5584105a-584a-1d86-db1c-636193e8c98e
---

![A photo of the MIT classroom in which 6.831 was taught.](BASEURL_PLACEHOLDER/resources/ac6-1) This activity is intended to get you thinking about the user-centered design process, by conducting a very lightweight UCD process on a few problems in our classroom.

1\. Screen Locations
--------------------

The first problem we'd like to solve: where should the slides be projected in the room? Recall that UCD has three parts.

**Early focus on users and tasks.** Let's identify the users of the room and their critical tasks (at least with respect to the slide projection problem).

> Who are the users of the classrom? It's easy to see by observation that we have two main user classes: **students** and **teachers**.
> 
> What are their tasks? At a high level, students are here to **learn**; that's their goal. The teacher is here to **teach**. But we can unpack these high-level goals into more specific subtasks (choosing only the ones relevant to slide projection, for now). In order to learn, a student needs to **read slides**. The teacher needs to **show slides**.
> 
> This leads to one basic requirement for our problem: **Every student must be able to read the projected slides.**
> 
> We'll learn more about how to do user and task analysis in a future lecture, but this quick sketch will serve for now.

**Iterative design with prototypes.** How can we build prototypes of the slide projection, so that we can explore the design space before actually installing screens and projectors?

> The simplest prototype we might build is a **map of the room**, showing where the seats are and marking where the screens might be. We can use this "prototype" to check sight lines and distances. You may not think of a mere sketch as a prototype, but it is—it's a physical realization of an idea, and we can apply tests to it and evaluate it.
> 
> But it's a weak prototype. The next prototype we might do is to simulate screen projection in the room itself, by holding up posters or drawing on the walls. Then we can evaluate it with real people sitting in the room, telling us what they can or can't read.
> 
> An even higher-fidelity prototype would bring in portable LCD projectors and temporary screens (or big white sheets) to hang on the wall, in order to project actual slides.
> 
> Finally, we might do a permanent installation—which is no longer a prototype really, but a full-blown, expensive implementation.

**Empirical evaluation throughout the iterative process.** How can we evaluate the protoype to provide data and insight for the next iteration?

> Suppose we fill the room with people (like now) and draw some simulated slides on the whiteboard. Now we can run usability tests. Some of the tests might be quantitative: "How many people can read this?" "Write down all the words on the screen as fast as you can." Others might be qualitative: "Is this comfortable to read?" "Are you craning your neck?"
> 
> We might even find, on evaluating prototypes, that we left out important requirements: **Every student must be able to see where the teacher is pointing on a slide. The teacher must be able to see the students' faces.** Because we used cheap prototypes, however, we didn't invest a lot of resources in an implementation that we have to change or throw away—or worse, never fix.

2\. Pointing at the Screen
--------------------------

Now it's your turn. Let's fix the problem we just discovered: when the lecturer points at one screen using a hand or a laser pointer, students watching other screens don't see it.

**Early focus on users and tasks.** Who are the users? What are their tasks? What requirements does the system have? (Focus just on this narrow problem for now, not on everything that happens during class.)

**Iterative design with prototypes.** Suppose we'd like to solve this problem using computer vision to watch what the lecturer is doing and display a simulated pointer on the other screens. Imagine a few ways this solution could be prototyped. Implement and use one of them right now.

**Empirical evaluation throughout the process.** Evaluate your prototype (qualitatively). What did you learn about the problem space? How might you revise the design in response?

3\. Students Pointing at the Screen
-----------------------------------

Now suppose this is a distance learning class, so the lecturer isn't in the room with the students. The problem is that when a student wants to ask a question about part of a slide, the lecturer can't see where they're pointing.

**Early focus on users and tasks.** Who are the users? What are their tasks? What requirements does the system have?

**Iterative design with prototypes.** Suppose we'd like to solve this problem by embedding one flat panel touchscreen display in the middle of every table, showing the current slide, which students can press with a finger to show a cursor on the slide. Prototype this solution and try your prototype right now.

**Empirical evaluation throughout the process.** Evaluate your prototype (qualitatively). What did you learn about the problem space? How might you revise the design in response?