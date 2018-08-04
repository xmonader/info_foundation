# Trello Usage

![@https://images.unsplash.com/photo-1494074734099-c4ec0c45687a?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=f18b2bf25abbaeddbe5ea1f9dae1ff85&auto=format&fit=crop&w=1950&q=80](trello_usage.jpeg)


**Make sure every board is defined in** the [circles document](circles.md)

## The Info Card

example https://trello.com/c/o8VWFzcH/23-info

is one special card which should be there on each trello board, it has the links to the info related to this board.

e.g. links to circle page, link to gdrive, link to other trello boards relevant, ...
e.g. info about timing (needed for e.g. trello roadmap board)

## different types of trello boards


### funnel board

- storyboard name: $teamname_funnel_$region or $teamname_funnel if no region e.g. tfgrid_funnel_africa
   - teamname is without _
- swimlanes
   - new          : first contact, validating opportunity
   - interested   
   - confirmed    : email or oral confirmation that they want to do the deal
   - negotiation  : working on the details, contract stage sits in here
   - won          : all docs done, waiting for e.g. payment, delivery, ...
   - idea         : should we contact & continue with the prospect
- when story won & paid, just archive, when story lost just archive

use labels for

- urgency e.g. red (when more urgent just move to top of list, red/orange is to promote even more)
- named labels can be used for e.g. region, ...  (free to select)
- there needs to be a chat attached to each funnel board

### stories board

- stories are about groups of people working together, there need to be regular meetings
   - boards are used to organize work over defined intervals
   - do not copy info from funnel or roadmap board
- storyboard name: $teamname_stories_$name e.g. tftoken_stories_promotion
   - teamname is without _
- [how to write a story](stories.md)
- board owner
   - calls meetings when required
   - communicate with board members to help them with communication, ...
- story owners
   - owns the story and makes sure is executed in time & done following all requirements
- swimlanes
  - this_week
  - question_blocking
  - this_month
  - this_quarter
  - verification (needs to stay in here till at least board owner approves)
  - future
- when story done or no longer valid just archive
- stories can have tokens attached to them
   - create checklist call: token_bounty add people on there with token amount & lockup period e.g. 10000_oct_19
- there needs to be a chat attached to each stories board

### roadmap board

roadmaps are about content (feature requests, issues, ...) which need to be executed in a certain version of a delivery of a product or e.g. a website

- storyboard name: $teamname_roadmap_$name e.g. tftoken_roadmap_web
   - teamname is without _
   - web would be for wiki & websites
   - e.g. tftech_roadmap_archive
- swimlanes
   - $version
   - for the first to be delivered version use $version/$version_question/$version_done 
       - in other words the next version to be delivered has 3 swimlanes attached to it
   - do not have more than 3 versions active
   - the last one = 'future'
 - the focus here is on the content of the feature, issue and the version its not a story or a task !!!
 - the story owner = makes sure that the feature will be done in the right version
 - there needs to be a chat attached to each roadmap
 
