# Design notebook entry

## Last week's critique

**TODO:** Fill in this part with a summary and reflection on the critique you received for
last week's work. Answer questions such as:  How, specifically, did the feedback help
improve the project? Did the feedback point out or offer something you hadn't considered?
Did it help you make a design decision? Was it helpful in addressing the most pressing
issues in your project? How will you incorporate the feedback into your work? Will you
change something about the design, implementation, or evaluation as a result?

My feedback partner provided super helpful comments that helped me refine my roadmap for my project, and answered my questions that I had about areas I was unsure how my project would be structured. Specifically, they reinforced my desire to add a recurrence feature to my DSL as they noted that this would find this to be a useful feature too. However, they agreed that this aspect of my DSL may be harder to implement than other tasks that I want to complete. So, they suggested that I may want to save this implementation as a stretch goal after I have the core aspects of my DSL up and running. When making this comment, they also took the time to briefly go through an icalendar file they had on their computer and take note of the syntax. I thought that this was an extremely helpful aspect of their feedback as they pointed out to me that there are recurrence flags that can be set within the icalendar documentation. This made me feel less worried about tackling my most desired stretch goal, as my feedback partner helped point me in the right direction to complete this task.

Also, in Monday’s studio time, my partner and I took the time to explain our projects to each other. At the time, I had a lot of unanswered questions about the direction I would take the project and the details I would need to consider in order to make it happen. My feedback partner did a great job taking in all of the information I gave her about my project and suggesting the direction I should take things. In particular, I mentioned that I was unsure if I wanted my program to generate a calendar in google calendar, an excel spreadsheet, or in HTML. My partner considered this question that I was debating and informed me about Scala wrappers that were created specifically for excel sheets, and provided links for me to check them out. This helped me address one of the most pressing questions that I still had about my project, as I now have decided to go the excel sheet route. I really appreciated this piece of feedback as I did not know about the Scala wrappers which I will benefit greatly from.


## Description

**TODO:** Fill in this part with information about your work this week:
important design decisions, changes to previous decisions, open questions,
exciting milestones, preliminary results, etc. Feel free to include images
(e.g., a sketch of the design or a screenshot of a running program), links to
code, and any other resources that you think will help clearly convey your
design process.

This week, I feel like I made excellent progress on my project. The goal I initially set out to take on was to fully map out my project and make the important design choices for how I will structure my project. The week before this past week, before I made any progress of my own, I had a conversation with professor Wiedermann about my project plan; I wanted to get his opinion on if my project seemed feasible and how I could best shape it to the goals of this class. He provided me with great advice on how to structure my project. Namely, he suggested that I split my project into two DSL’s, one that handled events and another that dealt with the look and feel of the output. He also informed me about two super helpful tools that will be essential to my project- icalendar, and ical4j.
This week, I started by making the important design decisions which was my initial goal in my project plan. I decided that I would write both of my DSL’s externally and in Scala. After that, I wrote some sample syntax that I might be interested in implementing, which was inspired by other calendar DSLs that I found online. 
<picture>
With this out of the way, I moved onto more specific components of how my project would work- how I would integrate icalendar and ical4j. To do this, I started by doing a deep dive into these libraries and learning how they worked and what would be useful in the scope of my project. Although this was probably the least enjoyable aspect of my project work this week, I think that it was absolutely necessary for me to do. After this, I found that I had already completed the milestone that I set for myself in the project outline and was motivated to do more. 
I decided that in order to set myself up for the following week, where I will be writing the event handling parser, I should first get the ical4j library working in Scala. My new goal for this week was to write Scala code that used ical4j to create and add an event to an icalendar file. This task was harder than I expected it to be since there wasn’t any information online about how to use ical4j in Scala. At many moments I felt stuck and like I would not be able to figure out how to implement this myself without help. This was mostly because there were a lot of resources for how to use ical4j in Java but none for Scala. This required me to first understand how the Java code worked and then rewrite it in Scala. After I wrote code that I believed to work properly, I ran into a lot of issues adding the ical4j library dependencies to my build file. This tripped me up for a while because I was unsure if I was having issues importing the library or setting up the dependencies correctly. However, after a lot of error handling, I was able to produce an create and add an event to an icalendar file. 

Starting next week, I will decide what else I want my icalendar file to include and devise a way to parse my current output.


## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

My current most pressing issue is where I will get started with my project: getting ical4j up and running in scala. Since I never have done this before, I can foresee it potenitally taking me a decent amount of time to figure out and get working properly. I will keep my progress on this task updated here.
1. 

**What questions do you have for your critique partners? How can they best help
you?**

**How much time did you spend on the project this week? If you're working in a
team, how did you share the work?**

**Compared to what you wrote in your contract about what you want to get out of this
project, how did this week go?**
