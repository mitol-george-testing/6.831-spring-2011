---
content_type: page
parent_title: In-Class Activities
parent_uid: 09700340-607a-547c-da2b-20b3c55a84bd
title: Input/Output Technology
uid: ee31b351-36ae-e855-708e-233bdef03182
---

The purpose of this activity is to experiment with ways to do background processing in graphical user interfaces. You will need to look at [LongRun.java](/ans7870/6/6.831/s11/LongRun.java), which is the Java code you'll be using. It's compiled into [LongRun.jar](/ans7870/6/6.831/s11/LongRun.jar).

Long Task in Event Handler
--------------------------

Run the Java program. You'll see a counter, initially at 0. The job of the long task is to increment this counter by 1000 units (and simulating computation or I/O by spending about 1 millisecond to do each increment). So the correct behavior is that you should see the counter rapidly increase from 0 to 1000.

Press the Event Handler button. What actually happens? Look at the code. Why does it have the effect you saw?

Long Task in Thread
-------------------

Now click the Thread button, and examine the corresponding code. What happens?

Now click the Thread button several times quickly, so that several threads are running at the same time. After all the threads are done, you'd expect to see the counter increase by some multiple of 1000. What actually happens? Why?

Using invokeLater()
-------------------

Now load [LongRun.java](/ans7870/6/6.831/s11/LongRun.java) into Eclipse or an editor, and modify the code for the UsingInvokeLater button so that it calls SwingUtilities.invokeLater() to avoid the problem you saw with the Thread button. There's an example of the syntax for invokeLater() elsewhere in the program.

Click the UsingInvokeLater button a few times quickly to make sure you fixed it, and make sure the counter still increases steadily over time instead of skipping straight to its final value.

Using Timers
------------

Now implement the body of the UsingTimer button so that it uses javax.swing.Timer to do the work in the background.

Look at your console, which displays the actual time that the background task takes. The task should take about 1000 milliseconds; any extra is overhead. Compare the overhead of your InvokeLater with the overhead of your Timer. Can you get them both down around 1000-1100 milliseconds?