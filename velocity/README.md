# Velocity

## Story points over time

But not wall clock time. It's based on the constraints of the individuals that make up your team.

Velocity is calculated using your capacity. And your capacity is a calculation of time. But velocity does not necessarily reflect how much time the team spent working.

Velocity is a measurement of how much meaningful, working software the team is able to produce. If your velocity is low, it *might* mean the team is lazy and didn't do their jobs. But it could also be caused by a number of other reasons.

For example, tech debt in your existing code base can cause unexpected failure cases and late stage bugs. You don't score bugs, because bug fixes don't reflect *meaningful working software*.

As proof by contradiction, consider what would happen if you did score bugs. Say each one got estimated as 2 or 3 or 5 story points. And suppose your team introduces a handful of bugs, then fixes them all at once.

If you give yourselves credit for each one that you fix, you can quickly rack up an impressive *velocity*. But in that case, **have you really accomplished anything?**

Intuitively, bugs should produce a **slow-down** of the teams velocity, not an increase.

So we won't score bugs. Instead, velocity will only go up when we complete user stories. And we don't consider those user stories *done* until the product owner has reviewed them and signed off that they are working as expected.

"But wait, doesn't that put a lot of veto power into the hands of the product owner?"

Anyone who has been in the software industry has heard "That's not what I meant!".

We need a mutually acceptable way to unambiguously decide "When is a user story actually *done*?"

To solve that problem, we turn to [acceptance criteria](../acceptance-criteria)
