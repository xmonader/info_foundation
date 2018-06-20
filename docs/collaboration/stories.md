# Stories

![](https://images.unsplash.com/photo-1456324504439-367cee3b3c32?ixlib=rb-0.3.5&s=45160e59ac36a57dce0ec249a7b75161&auto=format&fit=crop&w=1350&q=80)

Stories help us to organize our work. They need to comply to certain requirements to be effective though.

A story normally represents the view of a person, e.g. "I as product owner for product X would like to see Y features to be implemented because... customer Z needs this... our strategy is..."

Writing user stories may seem to be simple but there are many ways you can mess it up (incomplete, inconsistent or missing valuable parts such ass acceptance criteria/DOD), to avoid this common mistakes, We have created this list of the most common pitfalls you must avoid while creating your stories.  [see the story pitfalls](story_pitfalls.md)

Stories are pieces of work (not simple tasks) which are aggregated in a story = its like a card you would stick on a whiteboard.

Stories are the cards as used in story_boards in trello: see [trello_usage](trello_usage.md)

## Properties

- Well chosen name
- Clear description of what we want to achieve
- Some minimal description of deliverables and requirements (don't write specs here, they are markdown docs see below)
- Story Card owner:
    - best to only have 1, is linked to the story
- Estimation of the effort in days or hours (optional)
    - this needs to be redone on max 2 daily basis by story card owner
    - best to put this in title e.g. [2d] or [8h]
- A story needs to have a beginning & an end
- A story should never take longer than 1 month, if it is longer create 2 stories.

- optional: define a priority = a label
    - Critical (Red)
    - Urgent (Orange)
    - Normal (is no label)
    - Minor (Green)

- Milestone: 
    - the swimlane in the story board (is the vertical column) 
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

- The time estimate is in title, this is the remaining time for this story
    - this is only set by the story card owner !!!
    - this needs to be set on max 2 daily basis !!!
    - time is working time (sum over all people)
    - this is an estimate - this is not the sum of the times used inside the story or specs underneath

## Body

requirements & remarks are optional.


```
## GOAL:

Clearly describe what needs to be achieved.

## DESCRIPTION

Describe what story is about.

## REQUIREMENTS:

- very high level overview and/or links to requirements (which are in code repo)
    - only the high level overview, the rest is in the code repo's

## REMARKS:

- List all remarks
 
```

