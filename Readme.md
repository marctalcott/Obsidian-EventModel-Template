
# Use case:
As the owner of a food truck, or a mobile farmers market, I would like to track the history of my events and locations and sales. This will help me in planning for the next year better for higher profits.

#### We will track items such as:
- Event Dates
- Event Hours
- Booth rental costs
- Sales per interval of my choosing (hour, day, event)
- Number of sales
- Average sale price


We will want to add new feature in the future and the above features may change during development (don't they always?), so we want our code to be flexible to changes.

# Architecture:
This application has enough complexity that it is a viable candidate for [[CQRS]] and [[Event Sourcing]].  It could also be written in a standard [[Layered Cake architecture]].  I expect this to be the start of an application that will grow and expand in the future, therefore I want to make sure I invest the time in a proper architecture.

Layered Cake projects are easy to start and and work well for quick projects, but I have learned that Event Sourcing with CQRS works better in the long run as more and more changes are requested. It allows us to add features at a constant rate, while the Layered Cake architecture leads to increasing complexity over time.

Once you become familiar with both approaches, the advantage that Layered Cake has for start up time diminishes.  We can get up and running with CQRS and Event Sourcing just as quick if not quicker.  This is because with any established architecture, we tend to start projects by copying the best parts of our infrastructure from a recent project.  If you are writing all that by hand every time you are really wasting time, and losing built up knowledge.
# Documentation:

Documentation is useful for all stages of the software lifecycle.  We will create a [[Mobile Market Event Model]] as our core documentation because it provides a flexible solution that grows with the software. [[ Event Modeling]] is a technique created by Adam Dymitruk and is the best method I've seen for describing how software works to both end users and developers.  This little book will teach you how we use Event Modeling in great detail.

We will need User Stories for our developers. Event modeling gives us built in user stories. 

Once the software is up and running we need documentation of that can be used for User Guides and for training new  developers how the current application is expected to work. This is helpful when there are bugs and they aren't sure what the correct behavior should be. 
The Event Model can do all this. Additional docs can summarize the Event Model in various ways depending on the audience.



# Obsidian-EventModel-Template
# Obsidian-EventModel-Template
