## Development

### How we work

- [Packaging](../development/packaging.md)
- [Contributing](../development/contributing.md)
- [Staging Environment](../development/staging.md)

## Releases

Instructions for creating a release are [here](../development/release.md).

### Cadence

FlowForge is released every four weeks, on a Thursday. There's 13 releases each
year. The initial release is scheduled for the 20th of January. This implies:

v0.2 is scheduled for 2022/02/17

v0.3 is scheduled for 2022/03/17

### Planning

We use GitHub issues for planning the work in a release. A Milestone should exist
for the current release (N) and the next one (N+1). We do not schedule work beyond
that as priorities can change through a release.

There are three types of issue used for planning work:

 - **Epic**: a significant feature or piece of work that doesn't easily fit into
   a single release. It will typically have a number of Stories
   and/or Tasks associated with it that can be delivered iteratively.

 - **Story**: a *user-oriented* description of a feature. It should describe what
   a user should be able to do and identify the value that brings to the user.
   A story should be deliverable in a single release.

 - **Task**: a piece of work that isn't necessarily tied to a specific Epic or Story.
   For example, items related to technical debt or house-keeping chores.

A planning meeting is held at the start of the release. In this meeting the team
discuss the current backlog of stories, tasks and bugs to propose items to be added
to the release. All items assigned to a milestone should have an assigned owner.

### Retrospective

The day after each FlowForge release, always a Friday, a meeting is scheduled
by the CTO. This meeting includes 3 parts: a retrospective on the last release,
complete scheduling for the next release, and kick off development for the next
release.

An action from this meeting is that a release manager is allocated for the next release, 
that person takes the action to create the next release issue from the template then assign it to them.

### What to work on

For each release a selection of epics is being worked on. When an epic assigned
to a milestone there will be developments to complete it, however it might not
be fully completed and closed in the assigned milestone.

Epics are assigned to one or more individuals responsible for executing the work
and keeping the epics up-to-date.

Stories and tasks are assigned by the assignee of the associated epic, depending
on how the work is distributed.

#### Milestones are overscheduled

As epics and stories are assigned to milestones, it's unlikely there's not
enough work to be done. On the flipside, this means that not all scheduled epics
or stories will be completed.

### Launch Lunch

To celebrate the launch of a new version of FlowForge, we organize a lunch on the
release day. Each team member is encouraged to order a lunch (Expensable up to 20$
per launch) and join a social lunch zoom call.


### Project Board
The project board holds all issues and PR's across all our repos.

Within the project board we use the following status's and move between them as shown.

**No Status** This is the default for all new issues, The Product Owner will validate them to remove duplication, and move to an appropriate next status.
**Backlog** All items not currently assigned to a milestone. It contains Product Items (Epics/Stories) that are prioritised by the Product Owner and Technical Chores (Tasks) that are prioritised by the CTO..
**In Design** Assigned to current or next mileston, work on the item is focused on design work. User Experience, Creating wireframe mockups, sketching public API changes and Database model requirements.
**Read**  This is the engineering backlog for the current or next milestone. Items in this state should have enough information in them for anyone to pick and start implementing what is described, person may or may not be assigned.
**In Progress**  Actively Being worked on, person MUST be assigned (This should be a relatively short list) DRAFT PR's should stay in this state
**Review**  Work is complete awaiting Review, PR's that have been reviewed can then be merged, once a PR is ready for review the associated issues/stories should be moved to this state as well.
**Done**  PR Merged, Issue closed, Once PR is merged branch should be deleted.


