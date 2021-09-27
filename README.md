# Regex-Lesson

While the concept of a regex expression can seem complicated, it's actually quite undertsandable once broken down into components! Also known as regular expressions, they are used to find patterns within a string. They can also replace a sequence within that string. 

We will be looking at a regex expression involving validating an email address:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

At first glance, quite intimidating! Let's break it down.

Anchors are what contain the expression, so ^ begins the expression and $ completes it. A quantifier tells us there is another sequence to be matched, so this is the + sign seen here. This is known as a greedy quantifier. {2,6} tell us the email address should have a minimum of two characters and a max of six. In javascript, a charater class is what JS uses to classify any digit from zero to nine - expressed as /d. There are three groups and three bracket expressions here. The first bracker expression, [a-z0-9_\.-], is case sensitive numbers a-z, numbers 0-9, periods, hyphens, and an underscore. The second expression, [\da-z\.-], contains periods, hyphens, and case sensitive characters. The third expression, [a-z\.], includes periods and case sensitive characters. Quantifiers: Greedy and Lazy. Lazy quantifiers will make the shortest match in a system while greedy quanitifiers will allow the system to expand as far as it needs to.


