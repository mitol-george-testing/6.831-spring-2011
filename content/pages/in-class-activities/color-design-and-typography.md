---
content_type: page
parent_title: In-Class Activities
parent_uid: 09700340-607a-547c-da2b-20b3c55a84bd
title: Color Design and Typography
uid: a8e39d06-ec18-90ae-7f22-3e5cf0165120
---

The purpose of this activity is to explore some of the principles and pitfalls of color design and typography.

Judging Color Schemes
---------------------

Choose a web page whose color scheme you **like or dislike**. If none come to mind, here are a few suggestions:

*   [Ask.com](http://www.ask.com)
*   [Google Advanced Search](http://www.google.com/advanced_search?hl=en)

**Write down the main foreground and background colors it uses.** Use simple terms like "dark red" or "pale blue". Qualitatively speaking, what are the hue, saturation, and value of each one?

**Judge the legibility of the color scheme.** Does foreground text have good contrast with background text?

**Evaluate it with a squint test.** What colors "pop out"? Are these colors used for parts of the page that _should_ attract notice?

**Evaluate it for color-blind users.** Use [VisCheck](http://www.vischeck.net/vis-check/) to look at the web page as a deuteranope would see it. (VisCheck can translate simple web pages straight from a URL, but for complex pages you may need to take a screenshot and submit it as an image.) How does it fare now for legibility and squint test?

Exploring Typefaces
-------------------

For this part, you'll need to use Mozilla Firefox with the [Firebug extension](http://www.getfirebug.com/) installed, so that you can tweak properties of font and spacing dynamically and see their effects.

Open up Firebug by clicking on the little insect icon in the lower right corner of the Firefox window, and use its Inspect feature to locate the paragraph below:

> Four score and seven years ago our fathers brought forth on this continent, a new nation, conceived in Liberty, and dedicated to the proposition that all men are created equal.
> 
> Now we are engaged in a great civil war, testing whether that nation, or any nation so conceived and so dedicated, can long endure. We are met on a great battle-field of that war. We have come to dedicate a portion of that field, as a final resting place for those who here gave their lives that that nation might live. It is altogether fitting and proper that we should do this.
> 
> But, in a larger sense, we can not dedicate—we can not consecrate—we can not hallow—this ground. The brave men, living and dead, who struggled here, have consecrated it, far above our poor power to add or detract. The world will little note, nor long remember what we say here, but it can never forget what they did here. It is for us the living, rather, to be dedicated here to the unfinished work which they who fought here have thus far so nobly advanced. It is rather for us to be here dedicated to the great task remaining before us—that from these honored dead we take increased devotion to that cause for which they gave the last full measure of devotion—that we here highly resolve that these dead shall not have died in vain—that this nation, under God, shall have a new birth of freedom—and that government of the people, by the people, for the people, shall not perish from the earth.

In Firebug's Style panel on the right side, pull down Options and choose Show Computed Style so you can see the paragraph's current CSS styles. The top part of the style list (Text) is what we're interested in. Right-click on the Style pane and select Edit Element Style so that you can tweak some of the parameters below and see how they affect the paragraph:

*   Change **font-family** to **Garamond**. (If you don't see a change, you may not have Garamond installed; try Arial or Georgia instead.) How does the color of the paragraph change when you change the typeface?
*   Change **font-size** to **12pt** and **line-height** to **12pt**. How does 12 point text on 12 point leading look? Loosen up the leading until you're happy with it.
*   Change **width** to **20em**. How does the paragraph look now? Adjust the width until it feels right to you.