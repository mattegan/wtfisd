wtfisd
---
######when the fuck is shit due?
######a simple deadline manager aimed at people with due-dates

##Use
---
adding a task is as easy as making a lame cliché, like "easy as pie"
    matt$ wtfisd add 9 tomorrow call mom+I think she loves me or something

if you're one of those totally spontaneous people, feel free to add a task that's due whenever or at no specific time on a specific day
    matt$ wtfisd add * friday lanudry+everything is getting kind of smelly
    matt$ wtfisd add * * hit the gym

and when you're ready, figure all your shit out by running the list command
    matt$ wtfisd list
    - 0 overdue
    = today
        incomplete
        - (uyug)       * - laundry
        - (ryvn) 11:59pm - webassign
                             reading week 4
        complete
        - (sqdd)  2:00pm - about face reading
                             part 1, chapters 1-7
    + tomorrow
        incomplete
        - (shlu) 11:59pm - webassign
                             chapter 3, homework 1
    + 1st friday
    + 2nd saturday
    + 3rd sunday
    + 4th monday
    + 5th tuesday
        incomplete
        - (uqdz) 11:00am - CS reading
                             finish chapters 8, 9, 10

to mark an item as complete, or to mark it as incomplete because you forgot something, use the done and jk commands
    matt$ wtfisd done uqdz
    matt$ wtfisd done sqdd

##other important stuff
- it's currently a script that utilizes python3 located at /usr/local/bin/python3, this is how I want it running on my system, but this may change in other commits, not sure how I want to deal with it yet
- you need to create a file somewhere on your system and change the WTFISDFile variable in the script, the first line of the file should be a number of your choice

##things left to implement
- a way to edit items
- more listing options, visibility of complete items, visibility of overdue items, a way to see a specific range of dates
- possible other output methods

##things that could be changed in code refactors
- everything
- a cleaner output formatting system, everything is just kind of hard coded now, maybe some super simplistic template system thing (everything needs a templating system right?)

