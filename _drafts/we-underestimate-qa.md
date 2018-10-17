---
layout: post
comments: true
title: We underestimate QA
typora-copy-images-to: ..\images
---

# We underestimate Quality Assurance

As an industry, I don't think we understand the value of Quality Assurance properly, we think of QA as a safeguard against those "pesky developers" who do nothing right, and even as developers ourselves we tend to think writing tests is easy and requires no proper thought, all that matters is that we get high code coverage, as if in some way saying we have over 80% code coverage is some sort of bragging right. Having high coverage does not make it automatically "good" coverage, nor the "right" coverage.



The point is, in some way, either as software engineers or as managers, we tend to look at quality assurance as an afterthought, something we "need" to have, an expense, an insurance policy, instead of something we "want" to have.



## Companies who chose not to have QA



You may be a startup, or you may have the best, most technically proficient of developers, you may have no hard deadlines, but if you don’t have QA, I bet your software does not work as well as it should. 

This may seem obvious, but it constantly staggers me the number of companies that intentionally choose not to have QA engineers, instead focusing on hiring “the best” developers. This may be a valid approach, but if you don’t have a recruiting process capable of finding unicorns in today’s recruiting market, your luck with this approach will yield non-optimal results, and that will most likely happen anyway, even if you do.

Your rock star/ninja/sensei developers have biases, and probably some kind of god complex (he is a rock star, after all..) which is why when he finishes any development, to him, it will always seem like it works beautifully. 

But I bet they have what I will for now call, the “developers tunnel vision”. This is a recurring condition in our lives as developers where we test the same feature over and over again while programming, to the point where we no longer pay attention to the context in which what we’re developing will execute, and so, our own testing will always work because we will unconsciously be testing the same “happy paths” over and over again. The job of the QA engineer is to understand and exploit the biases, because they know we have them, as well as understand the context of the particular feature he/she might be testing, and make sure everything works as it should.

Chances are, if your company relies solely on a senior development team and no QA to create software, I bet there are a lot of weird bugs in your application, even though on the whole the application “works”. They may not be major issues (or maybe they are) but no doubt a good QA engineer would make all the difference.





## Separating QA from Engineering



One of the worst experiences I've ever had as far as dealing with quality assurance goes, was when our quality assurance team was both physically and structurally separated from the rest of engineering. 

You can imagine the problems that arise from this, managers fighting and pointing fingers over bug reports (which, for some reason I still don't understand, always became a problem after 5:30pm, leading to both the development team and QA needing to work overtime/weekends often, to compensate the late detection of critical issues). 

There was also this constant need to be overly political about issues either the development team or QA found, since speaking directly with the involved parties was met with relative indifference and lack of urgency, because it was not a problem right now (and those report related issues were).

The long e-mail chains discussing what were the absolutely critical issues that needed solving for the next release, the inevitable delays, the back-and-forth ticket close and reopen due to “can’t reproduce”, the overall sense of lack of team spirit when working with people you don’t really know, never seen in person and just generally don’t care about, leading to an inevitable “us versus them” mentality, etc.

Maybe in some way, most of these issues were just lack of communication, but good communication does not come easy, or fast. It requires time, it requires knowing the people involved and understanding their priorities, it requires addressing the issues together, and all of this is extremely hard to to when you have management over your head, and fighting between themselves over a number on a report. 

A much better approach in my opinion is to just merge development and quality assurance under the same company entity, and have them work together in teams. This means your teams should have *x* number of developers, and *y* number of QA engineers, in whatever ratio your company sees fit, as long as it doesn’t overburden any of the specific team disciplines. 

With this approach, you eliminate the overhead of having to go through management to solve your problems, no fighting, no “urgent" meetings over critical bugs, no e-mail chains. Your team deliverables are the responsibility of your team only, and it is up to them how, and how fast, they will solve their own issues. Your developers and your QA’s will work on the same team, and share the same space, hopefully learning about themselves and their personalities in the process, which helps communication. 



## So what makes a good QA engineer then?



It depends on the particular needs of your project obviously, but I would argue that a good quality assurance engineer needs at least some of these traits:



1. **Knowing how to program basic software**

   By that I mean, there is no need to understand complex design patterns or having experience with software architecture schemes, but this person should know how to write a unit, and more importantly, an integration test.



2. **Be extremely detail oriented**

   Remember how previously mentioned a QA engineer should be able to detect a developer’s biases? Well, couple that with a high understanding of the project and a little bit of OCD about the software being “just right”, and you got yourself a winner.



3. **Friendliness**

   As weird as it sounds, chances are, as a QA engineer you will have to deal with people, and knowing how to deal with people is key when an essential part of your job is to tell other people just how bad they messed up. 



Sadly, most of the time the industry tends to think dragging a mouse around a screen pressing on buttons to maybe find one that breaks something qualifies as quality assurance. Sure, part of the job is to do just that, when a particular feature does not lend itself to proper test automation, but reducing such an important job to mouse clicking denies its greatness. A good QA engineer will write automated tests, will make sure your continuous deployment scheme fails as soon as possible, and will make sure the logging information collected has the necessary information for proper debugging. 



## Why is any of this important?



Ok, so you have a developers only team, and it creates good enough software, so why would you even care about having a QA engineer joining your team? 

Here’s why you should care, if your team has a good QA engineer you will start to notice a few things happening.



**Suddenly, and without you noticing, less critical bugs reach your production environment**

Because you hired a good one, he will now start creating proper unit/integration tests, or at the very least, creating the test specifications so that developers can code them. Meaning every new feature your application gets will at least not break previous code, and if you don’t value resilience in your software, I hope you at least value the developer hours you’d have to pay to have them try to figure out why changing a variable name in some random frontend JavaScript file is breaking the PDF export feature in your backend (or any other particular example you can think of…), in other words, a good QA **saves you money**.



**Your developers will get better**

Developers have egos, and we don’t like having other people telling us our work is less than perfect, so when the team’s QA engineer tells us we have a major bug in our code, you can be sure we will be extra attentive the next time we’re coding a similar feature.



**Your QA’s will get better**

Because you placed you QA engineer in a specific team, he or she will become familiar with your developer’s problems and will work with them to try to solve them, in the process acquiring a better understanding of your team’s specific context, as well as getting better at programming by learning from the team’s developers. This means going forward, your QA will write better tests, will identify corner cases quicker, and will be able to help your developers understand where the problem lies faster.



**Your team will deliver faster, and with higher quality**

Having someone command over the team’s testing procedures means new features get tested quicker, this means you will finder problems earlier, which means you will solve them faster, which means your developers get to move on to other features faster as well. This makes your team deliver more, and with better quality.





![The best of brothers](..\images\2kbqw6.jpg)





## Ultimately, It’s up to you and your company



There is not much I can do to convince you whether I’m right or wrong, and there are no absolutes when it comes to how teams should work. All I can really tell you is about my experience, I have worked on all of the situations I mentioned above, and there was a clear advantage to me in having someone who's experienced in my team, it helped me grow as a developer, I gained a much better understanding of why QA is important, myself and my team ended up doing much better work overall, and we got to grow together as professionals, which was honestly the best part in all of this.





