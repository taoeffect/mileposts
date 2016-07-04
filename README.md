# The Mileposts Methodology

Mileposts are special types of issues, similar to _[milestones](https://guides.github.com/features/issues/#filtering)_, but not as heavy and not (necessarily) bound to any specific release of the software.

### Purpose of a Milepost

In Mileposts, the _milepost lead_ saves the entire team energy _by clearly explaining what's going on_.

##### _Mileposts_ vs _Milestones_

- A milepost (MP) is _assigned-to_ and _managed-by_ a specific person: the milepost lead.
- Both milestones and mileposts aggregate _other issues_ together.
- Mileposts can contain issues that are assigned to a milestone, but a milepost does not need to be assigned to a milestone.
- Mileposts describe a specific _subarea_ of the project that has been claimed by the milepost lead (and those who may be helping them work on that subarea).

We include an example and a [specification](#the-milepost-spec) (for those who want one) below.

## Badge

Taking inspiration from [standard-js](https://github.com/feross/standard), you can include one of these badges in your readme to
let people know that your project is using Mileposts for its onboarding and project management.

[![mileposts](https://cdn.rawgit.com/taoeffect/mileposts/master/badge.svg)](https://github.com/taoeffect/mileposts)

```markdown
[![mileposts](https://cdn.rawgit.com/taoeffect/mileposts/master/badge.svg)](https://github.com/taoeffect/mileposts)
```

[![mileposts](https://img.shields.io/badge/onboarding-mileposts-brightgreen.svg)](https://github.com/taoeffect/mileposts)

```markdown
[![mileposts](https://img.shields.io/badge/onboarding-mileposts-brightgreen.svg)](https://github.com/taoeffect/mileposts)
```

## Milepost Example

See the [example milepost](https://github.com/taoeffect/mileposts/issues/1) in this issues tracker.

## Milepost Template

We recommend using **[saved replies](https://help.github.com/articles/creating-a-saved-reply/)** instead of [issue templates](https://github.com/blog/2111-issue-and-pull-request-templates) for creating Mileposts on GitHub.

Create a saved reply and copy/paste this content into it:

```markdown
Branch: **branch**

#### Description

A description of what this milepost is trying to accomplish, and the subarea (of
this project) that work on this milepost will restrict itself to. Make sure to
include @mentions of all collaborators who are (or may be) involved in this
milepost, and what their roles are.

#### Files

- Create `path/to/file`
- Remove `path/to/file`
- Update `path/to/file`

#### Issues

List of issues that need to be closed for closing this milepost:

- [ ] #29 - Brief description of issue #29
- [x] #30 - Example of an issue that has been closed
- [ ] #28 - Example of an issue that's shared with another MP **(shared with MP #50)**
```

Mileposts **must** be assigned to someone, called the **milepost lead**.

## The Milepost "Spec"

A milepost is an issue that has this format:

- **MUST** have a tag that is one of: `Milepost` or `milepost` or `MILEPOST`.
  - The tag's color **SHOULD** stand out from other tags (black or white are good choices).
- **MUST** use a title that represents the subarea being worked on.
- **MUST** be assigned to the milepost lead.
- **MUST** state the branch that's tracking the _latest progress_ for the milepost.
- **MUST** contain a description of the subarea that's being worked on.
- **SHOULD** state the (user)names of any other collaborators who are (or might) be working on this milepost.
- **MUST** contain a list of files that might be modified, created, or deleted.
  - **IF** a milepost shares files with another milepost, then that **MUST** be _clearly and explicitely_ stated (e.g. `(shared with MP #30)`).
- **MUST** have a list of issues (with checkboxes) that are being worked on as part of this milepost.
  - Each issue in the list **SHOULD** have a brief description (can just be the issue's title).
  - **IF** a milepost shares an issue with another milepost, then that **MUST** be _clearly and explicitely_ stated (e.g. `(shared with MP #30)`).
- **SHOULD** contain a roadmap describing what the plan is to close the milepost.
- **MAY** be assigned to a milestone.

Mileposts **SHOULD** contain comments of the following nature:

- Regular or semi-regular updates on the current status/progress of the Milepost.
- Contain information about who is working on what part of the milepost.
- Questions & answers from other existing or new contributors about the nature/status of the milepost.
