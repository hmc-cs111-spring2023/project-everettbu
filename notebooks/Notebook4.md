# Design notebook entry

## Last week's critique

**TODO:** Fill in this part with a summary and reflection on the critique you received for
last week's work. Answer questions such as:  How, specifically, did the feedback help
improve the project? Did the feedback point out or offer something you hadn't considered?
Did it help you make a design decision? Was it helpful in addressing the most pressing
issues in your project? How will you incorporate the feedback into your work? Will you
change something about the design, implementation, or evaluation as a result?

This past week, my feedback group provided me with information that proved to be more helpful than I could have imagined. When I mentioned to my group that I wanted to make my calendar more than one month long without writing an extremely long HTML file, Occam told me about a library that he uses called FullCalendar. This tool allows one to create a highly customizable javascript calendar that perfectly fits the needs of my project. After looking into it and its documentation, I was able to get the calendar interface up and running in my HTML code within an hour. However, the most useful aspect of FullCalendar was its ability to take colors as an input for the events that I was already able to add to my calendar. In the documentation, it had a parsing section that made my most pressing issue heading into this week super easy to implement. I feel like this tool has helped my project evolve into something that I will actually use next semester, which was my main goal when starting this project. 


## Description

**TODO:** Fill in this part with information about your work this week:
important design decisions, changes to previous decisions, open questions,
exciting milestones, preliminary results, etc. Feel free to include images
(e.g., a sketch of the design or a screenshot of a running program), links to
code, and any other resources that you think will help clearly convey your
design process.

This week I made some very notable changes to my project compared to the outline illustrated in my original project plan. Initially, I set out this week with the main goal of adding colors and styles (bold, underline…) to the events in my calendar. I started this task by writing the parser that could handle the optional input of colors and styles when events are passed in. When I got this working, my js array also contained the color and style specified by the user. However, this is where I hit a roadblock as I did not know how to translate this information into my HTML output. I then spent some time doing some research on how to parse the colors and styles into CSS, but did not find anything that was particularly helpful for my project. So after spending some time struggling, trying to figure out how to implement this feature, I decided to take a break and look into FullCalendar. 

At first, I was unsure if the FullCalendar library would be well suited for my project. I feared that it was too build out and would not work well with my DSL. However, once I got it set up with my project, I realized it was exactly what I needed to move forward. Not only did it provide a clean looking calendar output with accurate months and days, it also provided a super simple way to input events into the calendar. FullCalendar has a built-in .addEvent method that creates an event object to be added to the calendar. This was super great for my project because it was a super easy way for me to add colors to the events in my calendar. Unintentionally, I found a solution to the problem that I was trying to solve. Once I was able to get colors parsed into my calendar output I shifted to getting styles parsed too. This is when I realized that at the current state of my project, I didn't really need to add styles to my events. Initially, I envisioned that a user would want to be able to strike through elements that they had completed and bold important ones. However, on second thought, I decided that making the font bold was likely a feature that not many people would use and there are better ways to show completed events. Instead, I added a simple feature that allowed a user to click on an event and turn it gray once completed. I was super pleased with the way this worked in my calendar and how it looked.

Finally, I decided to shift my attention to a task that I had put on hold since the first week of working on this project: the remove function. When I started to think about how to implement this feature, I realized that it was no longer necessary in my DSL. If a user wanted to remove an event, they would just delete an entry in the text file. So, once I realized this, I started thinking about how I could make my DSL more user friendly and easier to use. I decided that moving forward, I want the user to be able to edit the text file within the HTML interface instead of having to re-run the program every time they want to make a change to the text input. This is something that I briefly looked into before deciding that it was a rather large task to complete and outside the scope of this project. 


## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

Moving forward, I think that there are a lot of additional features that could make my DSL more user friendly and helpful to use. For example, I think the next implementation issue that I would like to solve would be to handle recurring items. This is something that I intentionally put off because I knew that it would be a large task for me to tackle and I decided that it was more important for me to get a very solid basic version of my project working well. Getting a recurrence feature working will allow me to make DSL far more powerful and complex. I will definitely attempt to implement this feature over the summer. 

Also, something else that I would like to do is add a feature that would allow a user to pass in a txt file through the html interface. I am currently imagining creating a way for the user to be able to view the items in their calendar at any point in time and make edits to the events. This would be extremely helpful for the user when interacting with my program, and this idea is the reason I decided to scrap the remove feature.

**What questions do you have for your critique partners? How can they best help
you?**

I only have one general question for my critique partners- If you were to use my program next semester, which features do you think I should add? What features do you find the most/least helpful?

**How much time did you spend on the project this week? If you're working in a
team, how did you share the work?**

I spent roughly 7-8 hours messing around with my project and implementing things that would make it more likely for me to use.

**Compared to what you wrote in your contract about what you want to get out of this
project, how did this week go?**

In my project plan I wrote that I wanted to spend this week wrapping up any loose ends. So, I created a short list of things that I felt would improve the user experience of my program. 
To do:
- Colors/font added
- Try out full calendar
- Click to cross out items
I was able to do all three of these items and add additional features that came to mind as I practiced using my DSL.
