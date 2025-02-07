# react-interview
Collection of Questions for job interview in various programming languages

## Requirements

### Backend

* Store matched questions and answers
* Read-only so we don't have to deal with authentication, lol
* Serve up Q&As in a super simple API
  * Paginated option (How many in a page, default value + query param?)
  * GET `/questions`
    * `?items`: (*default: 1*) number of items to get
    * `?tag`: (*default: ''*) one or more tags to filter by, comma delimited. If empty, Q&As are chosen randomly from all tags
    * `?random`: (*default: true*) randomize the order of the Q&As
* Endpoint to config front end
  * GET `/config` tags and difficulties
* Needs to be able to run outside of Docker (JR can't run Docker on his computer)
  * Try to avoid needing to install and run local services
* Q&A:
  * 1 or more Tag
  * 1 Difficulty Rating
  
### Front end

* Read one or more Q&As from the API
* Display a Q&A flash-card style
* Display list of Q&As
* Answers should be hidden initially, user should interact with the Question to show its Answer
* Have a difficulty selector, support multi-select
* Have a category selector, support multi-select
