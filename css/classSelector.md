http://www.w3.org/TR/css3-selectors/#class-html

CSS examples:

We can assign style information to all elements with class~="pastoral" as follows:

*.pastoral { color: green }  /* all elements with class~=pastoral */

or just

.pastoral { color: green }  /* all elements with class~=pastoral */

The following assigns style only to H1 elements with class~="pastoral":

H1.pastoral { color: green }  /* H1 elements with class~=pastoral */

Given these rules, the first H1 instance below would not have green text, while the second would:

<H1>Not green</H1>
<H1 class="pastoral">Very green</H1>

The following rule matches any P element whose class attribute has been assigned a list of whitespace-separated values that includes both pastoral and marine:

p.pastoral.marine { color: green }

This rule matches when class="pastoral blue aqua marine" but does not match for class="pastoral blue".
