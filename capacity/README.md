## Capacity

Overall capacity for the sprint reflects how much time you have available.

This can take the form of a table. The first column is each person's name. The second column reflects how much time that individual can contribute to the sprint.

To figure out your capacity, you'll need to talk to the members of your dev team and also do some simple math.

Start by counting the number of days in the sprint. For a typical two week sprint, you start with 14 days.

Subtracting the two weekends leaves 10.

From 10, you want to take out any time when **everyone** is going to be unavailable. Holidays fall under that description. But you'll also want to account for any events that will take time away from the sprint. For example, all-day quarterly planning. Or agile training.

In addition to things like all-day training sessions, you should consider smaller chunks of time, like meetings. Try to account for any time when the team is not able to focus on development work.

Also, it's ok to break a day in half, if that seems appropriate.

Regardless of the reason for removing time from the sprint, you should have a number of days that will be taken out from the running total.

Let's consider an example dev team. For simplicity, our team has only three members. And let's say that two holidays fall within our example sprint.

This gives you the maximum number of days that any team member can have. 8, in this case.

For each individual on the dev team, you need two pieces of information:

- Excluding holidays, are there any days during the sprint when you are **not working**?

- What **percentage** of your working time is dedicated to this team?

Continuing with our example, David is 100% dedicated to this development team and doesn't have any planned time off during the sprint. Here's his capacity:

```

Name   |  Capacity
-----------------------------------
David  | 8 X 6 X 100% = 48 hours.

```

Notice that we converted from days to hours. This keeps the decimal point in a comfortable position.

We used 6 hours to do the conversion. This is a good starting estimate for how much time per day is spent on sprint work. Some time will be consumed by email, meetings, expense reports, getting coffee, human resources paperwork, etc.

Another team member, Phil, has a planned vacation that overlaps with three days of the sprint. When not on vacation, Phil will also be 100% allocated to this team.

Again, we started from 14 days, subtracted two weekends to get 10. Then two holidays yields 8. Phil's vacation makes 5. Here's his capacity:


```

Name   |  Capacity
-----------------------------------
Phil   | 5 X 6 X 100% = 30 hours.

```

Our final team member, Elijah, doesn't have any planned days off during this sprint. But he will be splitting his time 50-50 between this team and another one.

Here's his capacity:

```

Name   |  Capacity
-----------------------------------
Elijah | 8 X 6 X 50%  = 24 hours.

```

If you prefer symbolic manipulation to prose, the following equations might help make the mechanics clear:

```

days = weeks * 7

weekend days = weeks * 2

company days = days - (weekend days + company non working days)

individual days total = company days - (individual non working days)

individual hours total = individual days total * 6

individual hours allocated to this team = individual hours total * percentage * 0.01

```

Returning to our example, let's look at how it stacks up.

```
Name   |  Capacity
-----------------------------------
David  | 8 X 6 X 100% = 48 hours.
Phil   | 5 X 6 X 100% = 30 hours.
Elijah | 8 X 6 X 50%  = 24  hours.
```

Now let's sum to get total hours for the team, for the sprint.

```
    48
    30
    24
+
-------
   102
```

So our capacity for this sprint is 102 hours.

Note that this example used a small team and included both holidays and vacation, so your number will probably be larger. But that's the point of capacity, to look at how much of people's time you will realistically have available to get work done, so you can select an appropriate amount of work to do.

If you know your team's [velocity](../velocity), you can combine that number with your capacity to calculate how many story points you can pull into the sprint.
