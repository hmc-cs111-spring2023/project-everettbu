# Design notebook entry

## Last week's critique

**TODO:** Fill in this part with a summary and reflection on the critique you received for
last week's work. Answer questions such as:  How, specifically, did the feedback help
improve the project? Did the feedback point out or offer something you hadn't considered?
Did it help you make a design decision? Was it helpful in addressing the most pressing
issues in your project? How will you incorporate the feedback into your work? Will you
change something about the design, implementation, or evaluation as a result?

Last Monday in class, Phoebe reminded me of something that I wrote about in my project pitch but forgot to implement. Up until this past week, I had been handling inputs by prompting the user for an event through the terminal and having them submit their request there. I had implemented this feature into my DSL for testing purposes and completely forgot that I wanted to pass in files that contained multiple events. That very same day, thanks to Phoebe’s reminder, I made sure that my DSL could read inputs from a text file. 

She also provided me with some of her insight on the current state of my projects and helped talk me through some of the dilemmas that I was facing. She agreed that I should prioritize adding stylistic elements to events in my calendar and handle them in one request instead of two. Also, she agreed that I would likely find it easier to write my calendar output in HTML instead of attempting to deal with google sheets. This past week, I kept her comments in mind while I started the process of adding writing my second DSL and the actual calendar.


## Description

**TODO:** Fill in this part with information about your work this week:
important design decisions, changes to previous decisions, open questions,
exciting milestones, preliminary results, etc. Feel free to include images
(e.g., a sketch of the design or a screenshot of a running program), links to
code, and any other resources that you think will help clearly convey your
design process.

This past week, I was able to close up a few loose ends left over from last week, but more importantly I was able to get a working prototype of my project which I am super stoked about. I started this week off by changing the way inputs were passed through my DSL, from entering them into the terminal to passing them through a text file. This new implementation can be seen in the input.txt file which allows the user to pass in multiple events at once.

Up until this point, I hadn't really realized that I should first get my outputs visually in a calendar before I started making edits to their style. So, I shifted gears and actually decided to get my front end application working before writing my second DSL. By making this decision, I decided to swap the goals I set for myself in weeks 3 and 4. In Monday's class I ultimately decided that I would likely find it easier to create an HTML output rather than dealing with a google sheets api, even though I don’t have very much experience with HTML and CSS. Luckily, I was able to find an HTML monthly calendar online that matched my needs. Within a few minutes, I had a calendar for the month of January working in my repo. My next challenge was to add events to it. This is what it initally looked like:
<img width="1421" alt="Screen Shot 2023-04-16 at 3 35 24 PM" src="https://user-images.githubusercontent.com/64377136/232377983-660c1393-a6ab-4e3f-90a7-4af3fe24d961.png">

At first, I tried to devise a way to parse the .ics output that my calendar was producing but only found extreme troubles. I spent far too long before Wednesday's class trying to work around errors triggered by google chrome and attempting to parse the hard to read .ics file. In class on Wednesday I talked to prof Wiedermann and he suggested that I take a different approach and leave the .ics file alone. I then shifted gears and decided to store my events in a separate array that could hopefully help me create my second DSL that constructed my HTML file. Here is a diagram that helped me set the direction I planned on taking moving forward this week:
![IMG_5156](https://user-images.githubusercontent.com/64377136/232377943-a41ccc35-2a9a-4183-8dc7-94f256242c0b.JPG)

Heading in this new direction, I decided to look up ways to add items from an array to an HTML file. I found a clever solution that used id’s to set markers throughout the code where text could be passed into. Trying out this approach, I created additional rows of empty cells in my calendar that contained id’s of the dates that they corresponded to. Then, I also changed the array that I created to store my events from scala to javascript and made sure that the dates were stored in the same format as the date-ids in my HTML file.
<img width="373" alt="Screen Shot 2023-04-16 at 9 28 53 PM" src="https://user-images.githubusercontent.com/64377136/232378179-279fd516-53d1-4c63-be31-fa18aa33055a.png">
<img width="404" alt="Screen Shot 2023-04-16 at 9 29 20 PM" src="https://user-images.githubusercontent.com/64377136/232378306-abdb2b33-45bb-45c9-bd8a-d0651c095b64.png">

After an hour or two of debugging, I successfully added events into the HTML calendar in plain black text. I also tested out adding (blue, black) at the end of one of my events and found that it did not cause any issues; this is where I will start next week.
<img width="1410" alt="Screen Shot 2023-04-16 at 9 31 01 PM" src="https://user-images.githubusercontent.com/64377136/232378538-6ec66027-5ec1-4571-80c4-1ca141037526.png">


## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

**What questions do you have for your critique partners? How can they best help
you?**

**How much time did you spend on the project this week? If you're working in a
team, how did you share the work?**

**Compared to what you wrote in your contract about what you want to get out of this
project, how did this week go?**
