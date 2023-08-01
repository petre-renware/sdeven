<small>**SDEVEN Software Development & Engineering Methodology**</small>

Version: 7.0.9<br>
Release date: 230801

***

<!-- #FIXME drop when finished -->
![wip_under_construction](pictures/under_maintenance.png){ width="500" }



# Operational Meetings (SDEVEN.45-OPME)

**Table of Content**

[TOC]

## Preamble

This procedure treat production and planning meetings that take place in software development process.

!!! info "Agile SCRUM compliance"
    Procedure follow Agile SCRUM methodology recommendations for meeting types.

From this perspective the meetings has two important sessions (aka discussion panels, sections). These sessions should be clearly marked on meeting agenda, meaning should be clear from agenda level what is the *principal session objective*:

* **planning** for next with **`PLAN`** _code-name_[^PLAN]
* **review** of what was done with **`REVW`** _code-name_[^REVW]

Of course, in each session inherently can happen things of both types, but *the principal session objective* should be just one of them.


### The `sprint` event and process

Before discussing *OPME meetings* a brief description of *`sprint`* concept could be necessary.

The **`sprint`** term describe the process (named event in "_Scrum Guide..._") where ideas, things are put in practice. It is a normal `software development` process like any other one and has the following properties.

!!! tip "sprint properties"
    It is a fixed length event of one month or less to create consistency. A new `sprint` starts immediately after the conclusion of the previous `sprint`. All the work necessary to achieve the goals / objectives including its _planning_, _review_, _execution_, etc happen within `sprints`.

These properties determine the nature of *software development approach* which, by using `sprints` becomes an *iterative* and *evolutionary (spiral model)* one.





## Type of meetings

The **OPME** meetings can be first classified using 2 perspectives:

* *objective* (**`OBJ`** _code-name_[^OBJ]) that was shortly discussed in previously section and can be a mix but with clear sections (discussion pannels)
* *frequency* (**`FRQ`** _code-name_[^FRQ]) of repetition and *duration* (**`DUR`** _code-name_[^DUR]) of each one

The **OPME** meetings are highly thought out to fit into the previous classifications WITHOUT CREATING mixes within each class or at least MINIMIZING the mixes.

!!! note "OPME Meetings"
    The following types of meetings can be held:

    * **development planning** (**`devPLAN`** _code-name_) meeting (Agile SCRUM equivalent event: Sprint Planning)
    * **operational schedule** (**`devOPER`** _code-name_) meeting (Agile SCRUM equivalent event: Daily Scrum)
    * **operational review** (**`devREVW`** _code-name_) meeting (Agile SCRUM equivalent event: Scrum Review)
    * **product goals review** (**`prodREVW`** _code-name_) meeting (Agile SCRUM equivalent event: Scrum Retrospective)





## `devPLAN` development planning

This meeting has goal to plan the start and execution of a `sprint` which will call **`sprintPLN`** in next. Also should note that a (any) `sprint` has a specific / principal objective (keep ONE to make sure the sprint is sprint !!!) which will be called **`sprintOBJ`** in next.


!!! warning "`sprintPLN` CONSTRAINTS"
    A `sprintPLAN` must take into account the following *constraint assumptions* during its execution:
    
    * no changes will be made, especially changes that would endanger the `sprintOBJ`
    * established quality (factors) will not decrease
    * the `sprint` corresponding *CHANGELOG* is refined as needed
    * scope may be clarified and renegotiated with the Product Owner / Product Manager as more is useful *but having in mind first assumption*

But *where comes from* the `sprint`? Well it comes from an issue list, usually found on ROADMAP file or a shorter list, but ROADMAP is the preferred way, place and this is "the way" SDEVEN recommend.

Otherwise, a `sprintPLAN` is absolutely similar to any other software development plan regarding an issue that has *a clear and completely defined finality*.

All the good practices and  technical rules in software engineering, for example regarding maintainability, *must be considered* as in any software development plan made with maximum responsibility and care in observing the rules of software engineering.





## `devOPER` operational schedule

-#TODO_tbd... #NOTE review this section -------------- from HERE

The purpose of the Daily Scrum is to inspect progress toward the Sprint Goal and adapt the Sprint Backlog as necessary, adjusting the upcoming planned work.

The Daily Scrum is a 15-minute event for the Developers of the Scrum Team. To reduce complexity, it is held at the same time and place every working day of the Sprint. If the Product Owner or Scrum Master are actively working on items in the Sprint Backlog, they participate as Developers.

The Developers can select whatever structure and techniques they want, as long as their Daily Scrum focuses on progress toward the Sprint Goal and produces an actionable plan for the next day of work. This creates focus and improves self-management.

Daily Scrums improve communications, identify impediments, promote quick decision-making, and consequently eliminate the need for other meetings.

The Daily Scrum is not the only time Developers are allowed to adjust their plan. They often meet throughout the day for more detailed discussions about adapting or re-planning the rest of the Sprint’s work.

-#NOTE ------------------------------------------------ up HERE





## `devREVW` operational review

-#TODO_tbd... #NOTE review this section -------------- from HERE

The purpose of the Sprint Review is to inspect the outcome of the Sprint and determine future adaptations. The Scrum Team presents the results of their work to key stakeholders and progress toward the Product Goal is discussed.

During the event, the Scrum Team and stakeholders review what was accomplished in the Sprint and what has changed in their environment. Based on this information, attendees collaborate on what to do next. The Product Backlog may also be adjusted to meet new opportunities. The Sprint Review is a working session and the Scrum Team should avoid limiting it to a presentation.

The Sprint Review is the second to last event of the Sprint and is timeboxed to a maximum of four hours for a one-month Sprint. For shorter Sprints, the event is usually shorter.

-#NOTE ------------------------------------------------ up HERE






## `prodREVW` product goals review

-#TODO_tbd... #NOTE review this section -------------- from HERE

The purpose of the Sprint Retrospective is to plan ways to increase quality and effectiveness.

The Scrum Team inspects how the last Sprint went with regards to individuals, interactions, processes, tools, and their Definition of Done. Inspected elements often vary with the domain of work. Assumptions that led them astray are identified and their origins explored. The Scrum Team discusses what went well during the Sprint, what problems it encountered, and how those problems were (or were not) solved.

The Scrum Team identifies the most helpful changes to improve its effectiveness. The most impactful improvements are addressed as soon as possible. They may even be added to the Sprint Backlog for the next Sprint.

The Sprint Retrospective concludes the Sprint. It is timeboxed to a maximum of three hours for a one-month Sprint. For shorter Sprints, the event is usually shorter.

-#NOTE ------------------------------------------------ up HERE






## Notes and abbreviations used in procedure

[^PLAN]: `PLAN` describe a type of OPME meeting where *planning is the principal objective*

[^REVW]: `REVW` describe a type of OPME meeting where *review and actual situation analysis are the principal objectives*

[^OBJ]: `OBJ` acronym used to show the *principal objective* of a OPME meeting - can be `REVW` or `PLAN`

[^FRQ]: `FRQ` acronym used to show the *frequency* of an OPME meeting

[^DUR]: `DUR` acronym used to show the *duration* of an OPME meeting


