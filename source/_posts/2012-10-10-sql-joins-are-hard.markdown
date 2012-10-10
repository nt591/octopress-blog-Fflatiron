---
layout: post
title: "SQL joins are HARD"
date: 2012-10-10 16:18
comments: true
categories: SQL
---

Here at the Flatiron School, we're building out our own internal feedback tool, which is wonderfully named Feedbackadoro (if you disapprove, please yell at <a href="http://www.twitter.com/aviflombaum">Avi</a>). We started out by building the SQL tables and some practice queries, and I'm pretty sure I need a lot more work to understand JOINs...

<!-- more -->

Imagine for a moment that you have three tables - one for users of the tool, one for submitted issues, and one for submitted solutions.

Got it?

Great. Now, I had to establish a personal understanding of what the tool would be used for and get into the mindset of the consumer. I felt that, if I were using the tool, I would want to be able to search for questions that were marked as CLOSED and had submitted answers from an instructor of the class. I then wanted to SELECT the name of the user, the content of the issue and the content of the solution

Having to INNER JOIN all three of the tables was tough, I wasn't sure if order mattered at first - would I need to join the user table before the solution? It turned out that the mistake I had the entire time wasn't a mistake at all! I wrote a query that outputted a blank entry in bash, but I thought it was breaking. Turns out my query was asking for all issues submitted by instructors. My tables didn't have that issue at all, why would instructors ask students for help?

Turns out the hardest part of joins isn't implementing them, but understanding the question you're trying to solve.

Have you had trouble with joins? What kept you up at night?