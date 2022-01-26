---
title: "MATLAB is better than I thought"
date: 2022-01-08T15:34:00-05:00
author: Hamish Pierpont
draft: false
---

My first college programming class at the University of Florida used MATLAB as its instructional
language. This class gave science and engineering majors basic computing skills, and I absolutely 
loved it - writing programs felt like casting magic spells. I switched into the computer science degree program the next semester. However, I distinctly remember my frustration with
MATLAB as a language. Why did I need to define functions in a separate file? What's with this
`clc; clear;` business at the beginning of each of my scripts? Why is my code so incredibly slow?
With all the unearned confidence of a bright kid with no experience, I proudly looked down on MATLAB
and shit-talked it to any unfortunate soul who asked my opinion.

This was in early 2018. Fast forward to 2021. I am now far more seasoned, with four programming
internships and several excruciatingly programming-heavy courses under my belt. I still appreciated
languages like Python and Julia, but my enthusiasm is tempered - I now know that Julia's package
manager on Windows is excruciatingly slow, that Python's greatness is due in large part to its
ecosystem, and that both languages have plenty of warts.
I sign up for the last required class for both of my degree programs: numerical analysis. I look
through the materials for the class and see that the *lingua franca* of the class will be MATLAB.
Sigh. I download MATLAB with a student license and start working on the first assignment.

To my delight, it is an absolute *joy* to use. The built-in functions are incredibly useful and well-documented. The MATLAB console is packed with pertinent information. I am shocked to find that 
MATLAB has anonymous functions like every other well-designed language in 2021, so my first
assignment - writing solvers to find the zeros of (mathematical) functions using the bisection,
Newton, and secant methods - is incredibly easy with first-class functions. Sharing code between
files doesn't make you want to pull your teeth out - MATLAB 1, Python 0. MATLAB's default behavior 
of keeping variables local to a script in scope after the script terminates is probably bad for big 
projects, but it is absolutely wonderful for exploratory data analysis - you can quickly examine
your results, graph them if necessary or interrogate these variables using the built-in MATLAB
terminal, and even view array/matrix values in a quasi-spreadsheet with a click of a button. Most
of my performance qualms are solved by swapping loops with vectorized functions and my improved
knowledge of computational complexity and computer architecture.

To be clear, MATLAB is still a computing environment with serious problems. It costs money, whereas
R/Python/Julia cost none. It is not open-source. I still think the language itself is less ergonomic
than Julia, and a lot of MATLAB code is illegible due to its popularity with non-coders.
Furthermore, many of these benefits are not unique to MATLAB itself. A lot of the upsides stated
above come simply from having a REPL attached, which is also true for Python, Julia, and many other
languages. However, the MATLAB product impressed me as a tool for exploratory data analysis.

# Ok. Who cares?

More generally, I think people who code improperly dismiss programming tools because
1. they were less experienced the last time they used the tool,
2. the tool does not match the problem they want to solve, and
3. the tool is not in vogue with the programming intelligentsia.

Here is an incomplete exploration of these three points.

## Point 1

I wrote a lot of MATLAB as a 19 year-old programming novice; indeed, I probably had less that one-hundred
hours of programming under my belt when I started writing MATLAB for my intro class. I learned a lot
about good programming in those few months through experimentation and mimicking my excellent
professor Dr. Ira Hill. I also wrote a lot of slow, ugly, sloppy code, and I spent even more time
debugging and bandaging this mess, often during late nights in the library. Given that my brain is
basically stone-age ape hardware, I think I learned to associate MATLAB with having a bad time,
which negatively colored my view of it.

One of my pet theories is that part of the reason for the love shown to languages like Haskell and
LISP among enthusiasts is that fewer people write truly shit code in those languages. They're often
introduced to programmers who already have learned good habits, whereas languages like Java, Python,
and (in my case) MATLAB are often used for people's first whack at programming. I doubt this
explains most of the love FP people have for FP languages, but I think it's worth keeping in mind
that everyone has written an ugly thicket of branching and looping logic with six levels of
indentation in a vanilla language like Java, and the pain of debugging that is still
there in your brain somewhere.

## Point 2

I stated above that MATLAB is a good tool for exploratory data analysis and scientific
modeling. I would *never* reach for it to make a desktop application; I'm sure it could be hacked
together to fit that mold, but why anyone would do so when we have Java and C# beats me.