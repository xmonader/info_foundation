# Stories

![@https://images.unsplash.com/photo-1456324504439-367cee3b3c32?ixlib=rb-0.3.5&s=45160e59ac36a57dce0ec249a7b75161&auto=format&fit=crop&w=1350&q=80](stories.jpeg)


Stories help us to organise our work. They need to comply with specific requirements to be effective.

A story normally represents the view of a person, e.g. "I as product owner for product X would like to see Y features to be implemented because... customer Z needs this... our strategy is..."

Writing user stories may seem to be simple, but it requires attention. Common mistakes include creating stories that are incomplete, inconsistent or missing valuable parts such ass acceptance criteria/DOD. To avoid this common mistakes, we have created this list of the most common pitfalls you must avoid while creating your stories.  [See the story pitfalls](/collaboration/story_pitfalls.md)

Stories are pieces of work (not simple tasks) which are aggregated in a story = its like a card you would stick on a whiteboard.

Stories are the cards as used in story_boards in trello: see [trello_usage](/collaboration/trello_usage.md)

## Properties of a "good story"

- Well chosen name/title
- A clear description of what we want to achieve
- A minimal description of deliverables and requirements (don't write specs here, they are markdown docs see below)
- It's preferably to only have 1 owner per story. You can link people that is part of the story but story owner needs to be on the title (see example below)
- Estimation of the effort in days or hours (optional)
    - this needs to be redone on max 2 daily basis by story card owner
    - best to put this in title e.g. [2d] or [8h]
- A story needs to have a beginning & an end
- A story should never take longer than 1 month, if it is longer create 2 stories.

- Optional: define a priority = a label
    - Critical (Red)
    - Urgent (Orange)
    - Normal (is no label)
    - Minor (Green)

- It has a milestone: the swimlane in the story board (is the vertical column) 
        - e.g. this_week, future, this_month

- tasks from a story are a checklist in the story

- Format:
	- Title: ```Story title``` [```time left e.g.4d```] e.g. Onboard the first 100 guardians [10d]



**Use links to put structure in story**

- Links For Non Product Related Story (URLs) to
    - Specifications (link to wiki, source = markdown document)
    - Questions/Bugs/FR (links to issue on EE)
    - Tickets (links to issue on EE or to trello cards in other non story board)
- Links For Product Related Story (URLs)  to
    - Specifications (requirements, code examples, ...) (in code github repo as markdown document)
    - Features or bugs which are related to the story (in code github repo as markdown document)

## Format

#### Title: ```$storyDescription``` ```[$time]```

- The time estimate is in the title; this is the remaining time for this story
    - this is only set by the story card owner !!!
    - this needs to be set on max 2 daily basis !!!
    - time is working time (sum over all people)
    - this is an estimate - this is not the sum of the times used inside the story or specs underneath

## Body

Requirements & remarks are optional.


```
## GOAL:

Clearly describe what needs to be achieved.

## DESCRIPTION:

Describe what story is about.

## REQUIREMENTS:

- very high level overview and/or links to requirements (which are in code repo) the rest is in the code repo's

## REMARKS:

- List all remarks
 
```

![Example of a "good story"](https://github.com/threefoldfoundation/info_foundation/blob/development/docs/collaboration/Example.png)
