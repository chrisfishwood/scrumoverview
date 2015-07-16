# scrumoverview

---

A high-level introduction to Scrum.

---

* Glossary:
  * **Stakeholders**: Any party interested in the application.  At a minimum, “the client”, the solution owner.
  * **Product/Solution Owner**: The SO/PO is the face of the client.
  * **Development Team (the team)**: People touching the code base (developers, UI/UX, etc.).  Traditionally, 7+/-2, but smaller teams work better for remote teams.
  * **Backlog**: Prioritized list of stories/epics that represent the stakeholders needs/wants.
  * **Sprint Backlog**: A subset of the Backlog that the team has *commited* to completing.
  * **Story**: A piece of work to be done.  Could be a chore, bug or feature.  Each story has an “Acceptance Criteria” that needs to be clearly defined.
  * **Backlog Grooming**: Done by the SO before sprint planning.  During this time, the SO makes sure that stories have as much clarity as possible and that the stories are in prioritized order.  This ensures that we can efficiently conduct Sprint planning.
  * **Scrum Master**: Protects the team from business interference and from themselves. Removes impediments, runs dailies/retros, captures metrics, does velocity analysis, story hour postmortem.  
  * **Sprints**: 1-4 week periods of time that stories are being worked.
  * **Capacity**: The number of development hours in a sprint.
  * **Velocity**: The number of points that a team completes in a sprint.
  * **Burndown**: The rate at which the team is having stories accepted compared to the Sprint Backlog.

---

### What is "process"?
At a high level, it’s the phases that a software system transitions though as it’s being modified.  At a more granular level, it’s the values, tools, ‘flows’ and information exchanges that are put in place by an organization when they are developing a software system.

### Why is process important?
Process is important because it adds structure to complex and chaotic events.  It defines development culture, it sets business expectations, it reduces risks and increases customer involvement.

* A few popular processes…
  * ~~Waterfall~~
  * Spiral
  * Prototype
  * Agile
    * eXtreme Programming
    * Scrum
    * KanBan
    * Lean software
    * ...

### What I’m talking about today.
Present a Scrum methodology that I used in a former life and list some of the pros/cons of it from both a developer and manager standpoint.  Make light recommendations around tweaking our process so that business’ needs are met.


### What is Scrum?
Scrum is an iterative and incremental agile software development methodology for managing product development. It's similar to our current process, but with a few differences in flow and responsibility.  Let's check them out.

![image](http://www.zenexmachina.com/assets/themes/zxm/images/page-artefacts/scrum-process-01.png)


### Sources:
* http://www.zenexmachina.com/
* https://en.wikipedia.org/wiki/Scrum_(software_development)

---

# Sprint Cadance

* Sprint planning:
  * SO has the backlog groomed based on SH needs.
  * Sprints tend to have themes associated with them.
  * Bugs, chores and features (anything that effects the team’s capacity) are all prioritized in the backlog.
  * Hotfixes, push X hours of work off the bottom of the backlog.  It’s the job of the scrum master to try to shield the team from these sorts of things.
  * SO has the teams velocity calculated for the sprint.  #ofFolks in the team * number of development days * 8 * .7 - team hours off.
  * The team starts at the top of the backlog, asks questions, gets definition and then estimates the stories.  Here the team “chooses” to pull the story for the sprint backlog.
  * Once the sprint backlog is +-10% of the team’s sprint capacity, the team chooses to commit to the sprint backlog.

* Sprint starts:
  * The sprint backlog is ‘locked’.
  * the stories are in prioritized order and should be worked from top to bottom.
  * Sprints can be aborted by the stakeholders or by the team, but there needs to be a damn good reason to do it as it causes swirl and messes with team morale.
  * The specific details of the development flow depends on how you want to track to effort.  But usually, it’s something like.
  “Start” the ticket, hack the codez, “complete” the ticket, log the hours that were worked on it.  QA picks up all completed tickets and tests them.  Once QA gives it a thumbs-up the ticket is “accepted” by the SO (not QA).
  * Daily standups, each team reports out three things: Yesterday, today, blockers?

* Sprint ends:
  * The SO accepts or rejects the sprint (not the client).  If accepted, the application is released.  If rejected, stories are created for it isn’t and the reasons for not accepting it as automatically added to the top of the backlog.
  * SO/SM runs the sprint review with the client.  The team members demo the stories that they worked on.  This fosters accountability.

-----------------------

#Pros and Cons

* Pros:
  * Communication is increased between development and business.
  * Goals are set at the beginning of a sprint and progress can be tracked via the project burndown, this means fewer surprises.
  * Time is tracked by all ‘team’ parties, so, in time, we should develop a good idea of the team’s velocity across sprints.
  * …this also has accounting benefits.
  * The Team is empowered by having a say on what is in the Sprint Backlog and is encouraged to push back on deadlines.
  * A planned approach forces you to finish dependencies in previous sprints (comps, spikes, etc.).

* Cons:
  * Additional diligence must be done but the SO (Brando) to make sure that Stories are impecibally defined with extremely terse Definitions of Done.
  * Hotfixes can be very disruptive.
  * Team morale can be more tumultuous (the accordion effect).
  * Time tracking can lead to a ‘do it quick, not right’ attitude, which leads to technical debt.
  * The team loses the freedom to self-prioritize chores for the greater good of the codebase.
  * Less pairing means less leveling-up.
