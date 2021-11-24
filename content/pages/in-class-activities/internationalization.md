---
content_type: page
parent_title: In-Class Activities
parent_uid: 09700340-607a-547c-da2b-20b3c55a84bd
title: Internationalization
uid: 55ad3551-4572-102b-d6bc-ab4bc7849322
---

The purpose of this exercise is to gain some appreciation of the problems of internationalization, specifically the wide variations in languages and scripts; bidirectional text; and the differences between character sets, fonts, and character encodings.

You will need Java installed on your laptop, so that you can run the sample program. You'll also need a modern web browser like Firefox/Safari/Opera, and a reasonably recent version of Windows, Mac OS, or Linux. Older platforms may have weaker support for i18n.

Internationalization
--------------------

Run the [CharacterEncoding](/ans7870/6/6.831/s11/CharacterEncoding.jar) program, just so you can see what its interface looks like. Then examine its code, [CharacterEncoding.java](/ans7870/6/6.831/s11/CharacterEncoding.java), particularly the main constructor for the class, with an eye for internationalization. What would need to be changed to internationalize it?

Character Encodings
-------------------

Now type some text into the box labeled Text. What do the other two boxes display?

Now copy the word **été** into the Text box. What do you observe?

Now visit this [Russian Wikipedia page](http://ru.wikipedia.org/wiki/IBM) and copy a word of it into the Text box. What do you observe?

Finally, visit this [Japanese Wikipedia page](http://ja.wikipedia.org/wiki/IBM) and copy a few characters of it into the Text box. What do you observe?

Bidirectionality
----------------

Visit this [Arabic Wikipedia page](http://ar.wikipedia.org/wiki/%D8%A2%D9%8A%E2%80%8C%D8%A8%D9%8A%E2%80%8C%D8%A5%D9%85) or this [Hebrew Wikipedia page](http://he.wikipedia.org/wiki/%D7%99%D7%91%D7%9E). How is the page laid out, relative to other Wikipedia pages?

Try to understand the effect of bidirectional text on editing by making selections. What happens when you select multiple lines? Notice that the page has English words embedded in it, like "International Business Machines." Make some selections that start in one language and end in the other. What happens?

If you have Firebug installed, you can use Inspect to highlight a paragraph, drill down into it in Firebug's tree display, and actually edit its text. Explore bidirectional editing by changing both the Arabic/Hebrew text and the English text. (You'll need to use copy-and-paste to simulate editing the Arabic or Hebrew, unless you know how to enter those characters at your keyboard.)