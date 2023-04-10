# Design notebook entry

## Last week's critique

**TODO:** Fill in this part with a summary and reflection on the critique you received for
last week's work. Answer questions such as:  How, specifically, did the feedback help
improve the project? Did the feedback point out or offer something you hadn't considered?
Did it help you make a design decision? Was it helpful in addressing the most pressing
issues in your project? How will you incorporate the feedback into your work? Will you
change something about the design, implementation, or evaluation as a result?

My feedback partner, Phoebe, was able to help me by providing some feedback about my syntax which is something I requested help with last week. I came into last week with an initial idea of how I would want the syntax to look/feel for the inputs into my DSL. After talking with Phoebe in class she, and the rest of my critique group, made some helpful suggestions that improved my initial draft. They suggested that I think about handling the keywords of my inputs as “verb-like” and “noun-like” to give it a natural language feel. For example, instead of writing ‘add Jan 15 “chapter 1”’ which was my original syntax, I decided to move the verb to the middle so that it reads ‘Jan 15 add “chapter 1”’. I found this suggestion extremely helpful as it gave me insight on what felt “natural” for others, and also it helped me refine my original idea into something that I prefer much more.

My feedback partner also noted that coloring and stylizing text should also be prioritized based on the sample output calendar that I am hoping my DSL will make easier to create. Even though I didn’t make any progress on this front this week, I definitely agree with her as it is a feature that will be a signature component to my DSL and make it actually something that will serve a purpose. With this in mind, I think that moving forward, I will add a little more focus to this task than I initially expected. Even though some of the features that I brainstormed in my project pitch would be cool and useful (a recurrence feature), I think that styling the inputs of my DSL is more important than I initially thought. It will be something I will make sure to add and implement to its fullest.


## Description

**TODO:** Fill in this part with information about your work this week:
important design decisions, changes to previous decisions, open questions,
exciting milestones, preliminary results, etc. Feel free to include images
(e.g., a sketch of the design or a screenshot of a running program), links to
code, and any other resources that you think will help clearly convey your
design process.

This past week I started to implement the parser for my first DSL (text input → ical file). Currently, it prompts the user for a text input in which they specify the month, whether they want to add or remove an event, and then the name of the event they want to manipulate. So far I only have gotten the add feature up and running (will talk about remove in a minute). Here is a screenshot of my program successfully adding an event titled call mom to an ical file. 

<img width="634" alt="Screen Shot 2023-04-09 at 8 36 45 PM" src="https://user-images.githubusercontent.com/64377136/230820669-6d0fa5f2-76a6-4da7-9eca-3ad90a54a70f.png">

I was super enthused when I was able to successfully parse my input for the first time as it was something I spent a lot of time mapping out and troubleshooting. A snag that I initially came across when implementing my parser was that I tried to create it in a separate file to make my code more organized. However, I did not really foresee that this organization effort would not be 100% necessary since the code that I wrote last week just created an ical file, all I needed to do was edit the code and add a parsing feature. Once I realized this, I started writing my parser by focusing on the add feature. When I started on this task, I quickly realized that it would be easiest for me to get started on my DSL if the inputs required a specific structure. This is where I made the design choice to structure my inputs as <month><day><verb><event> because it would make it easy for me to pick out the specific items I wanted to use. For example, my current version has a variable named “parts” that allows me to pick out the verb by calling parts(2). This was an implementation choice that took me a while to devise and it is something I am not fully sure if I want to keep. Nonetheless, it allowed me to functionally parse inputs where one wants to add an event.
  
After I completed this, I moved onto my remove feature that I anticipated to be a simple task. At the time, fully think through the fact that my code was not storing these ical files anywhere, all it did was create them. However, I still proceeded to write the remove feature as I felt like I was on a roll after successfully implementing add. To do this I chose to add a match expression in case I want to add more features later. So far, I haven't been able to test my remove feature this week as I have not created a way to store the ical files that I want to add to my calendar program. Working on this will be my first task for this upcoming week.


## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**
  


**What questions do you have for your critique partners? How can they best help
you?**

How would you approach saving my ical outputs so that they are easy to use when I start the application side of my project? I’m currently thinking of a simple array based structure but I would love to hear your thoughts. 
  
Something that I am considering working on for this week is making my input handling less harsh. For example, if I try to write “jan 14 add ‘chapter’” my program throws an error because Jan isn't capitalized. Do you think this is something that is something that I should prioritize or leave for later on?

**How much time did you spend on the project this week? If you're working in a
team, how did you share the work?**
 
I hoped to devote slightly more time to this project this past week but since I had multiple midterms I felt a little overwhelmed. Even though I didn't fall behind on my goal, this upcoming week I plan on making additional progress to put me in a better position to have a solid program by the end of the semester.
  
- Parser creation: 4.5 hours
- Notebook: 1 hour

**Compared to what you wrote in your contract about what you want to get out of this
project, how did this week go?**

In my contract I wrote “Week of 4/2: Write DSL #1, user --> icalendar” which is exactly what I got done this week. However, I will continue to build on the progress that I made this week and better complete the initial that I have running.

