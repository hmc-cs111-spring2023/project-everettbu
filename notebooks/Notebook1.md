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

This week, I feel like I made excellent progress on my project. The goal I initially set out to take on was to fully map out my project and make the important design choices for how I will structure my project. The week before this past week, before I made any progress of my own, I had a conversation with professor Wiedermann about my project plan; I wanted to get his opinion on if my project seemed feasible and how I could best shape it to the goals of this class. He provided me with great advice on how to structure my project. Namely, he suggested that I split my project into two DSL’s, one that handled events and another that dealt with the look and feel of the output. He also informed me about two super helpful tools that will be essential to my project- icalendar, and ical4j. (photo 1)

This week, I started by making the important design decisions which was my initial goal in my project plan. I decided that I would write both of my DSL’s externally and in Scala. After that, I wrote some sample syntax that I might be interested in implementing, which was inspired by other calendar DSLs that I found online. (photo 2)

With this out of the way, I moved onto more specific components of how my project would work- how I would integrate icalendar and ical4j. To do this, I started by doing a deep dive into these libraries and learning how they worked and what would be useful in the scope of my project. Although this was probably the least enjoyable aspect of my project work this week, I think that it was absolutely necessary for me to do. After this, I found that I had already completed the milestone that I set for myself in the project outline and was motivated to do more. 

I decided that in order to set myself up for the following week, where I will be writing the event handling parser, I should first get the ical4j library working in Scala. My new goal for this week was to write Scala code that used ical4j to create and add an event to an icalendar file. This task was harder than I expected it to be since there wasn’t any information online about how to use ical4j in Scala. At many moments I felt stuck and like I would not be able to figure out how to implement this myself without help. This was mostly because there were a lot of resources for how to use ical4j in Java but none for Scala. This required me to first understand how the Java code worked and then rewrite it in Scala. After I wrote code that I believed to work properly, I ran into a lot of issues adding the ical4j library dependencies to my build file. This tripped me up for a while because I was unsure if I was having issues importing the library or setting up the dependencies correctly. However, after a lot of error handling, I was able to produce an create and add an event to an icalendar file. Starting next week, I will decide what else I want my icalendar file to include and devise a way to parse my current output. (photo 3)

![IMG_5084 2](https://user-images.githubusercontent.com/64377136/229379187-775ebf85-ad11-4118-95bd-570eedd2426f.JPG)
<img width="708" alt="Screen Shot 2023-04-02 at 2 10 00 PM" src="https://user-images.githubusercontent.com/64377136/229379175-922869eb-ce88-4ca8-bea5-33f037cd38a4.png">
<img width="985" alt="Screen Shot 2023-04-02 at 2 17 13 PM" src="https://user-images.githubusercontent.com/64377136/229379455-569a9eba-fa8c-4f87-be9c-26ab2ff0b638.png">

## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

Looking forward to this upcoming week, my most pressing issue will be writing my first DSL and making the syntactical choices I will likely need to move forward with for the rest of the project. I am less worried about making the final decisions about my DSL’s syntax as I already have a solid idea of how I want my DSL to feel like. However, I am far more worried about writing the parser for my DSL as this was something I struggled with heavily on the Piconot assignment. I fear that this aspect of the assignment will take longer than just this week which is the goal I set for myself in my project outline. Ideally, I will combat this issue by thoroughly planning out how I want to attack this task and work on achieving something that works, not a super complex output at first. If I can do this, I feel that I will be able to add more features with ease and be at a good place to potentially meet the stretch goals I set for myself.

**What questions do you have for your critique partners? How can they best help
you?**

Like I mentioned in the previous question, I would benefit greatly from input on syntax choices that I will make for my DSL. At the moment, I just want to be able to add events in my own syntax but beyond that I am unsure of how I want my language to feel. Since my critique partner expressed a similar desire for my language, I hope that they will be able to provide insight for how they think my language should be structured. Should it feel more like a natural language? Aside from recurrence, what features are needed the most and which ones should I prioritize?

**How much time did you spend on the project this week? If you're working in a
team, how did you share the work?**

- Project plan/syntax design: 1 hour
- icalender/ical4j deep dive: 1 hour
- Writing initial example program: 3.5 hours
- Notebook: 1 hour

**Compared to what you wrote in your contract about what you want to get out of this
project, how did this week go?**

Like I mentioned in the description section, I think that this week went really well. I was able to meet the milestone that I set for myself in my project outline, and had time to go beyond this initial goal and get functional code written. As of now, I feel that I am at a great place moving forward into next week. However, I think that this next week I will likely need a little bit more outside assistance writing a functional parser, as this is something I’m not fully confident how to do. With this in mind, I am prepared to spend a little bit more time on the project this week since the task I set for myself is a little bit more challenging. 

