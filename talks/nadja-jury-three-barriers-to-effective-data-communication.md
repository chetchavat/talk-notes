# Nadja Jury: Three Barriers to Effective Data Communication
Coalesce Conference 2020

Link: https://www.youtube.com/watch?v=zFBfV-25dS4

## Intro
It's wild to have an idea for a talk and find one that basically covers all the points.


Working a lot in a ad-hoc basis, they found that data comms became a pretty big problem for them.

## Everyone should be speaking the same language
Not SQL vs Python, but speaking to each other about data with a shared understanding about the definitions.
- People should come to the data team with a simple question and get a simple answer, and not a series of follow up questions plus a lecture on how they might not be getting what they might be getting
- People should be able to talk to each other cross functionally without needed the data team to interpret the data presented by either team

We want to empower our colleagues to feel confident in the data.

## Three Barriers
- Stakeholder involvement
    - getting the correct people involved in the naming and definition process
- Engineering implementation
    - ensuring the data can be implemented in the data warehouse in a way that is good enough
- Discoverability
    - once data has been defined and implemented, anyone in the company can find them

Need to overcome all three barriers to achieve effective communication

## Stakeholder involvement
### Pre-Data team

#### Sales Team pipeline:
- Sales team defined a pipeline that made sense to them, but didn't have the ability to mark customers as their current stage due to technical limitation
- When Sales asks Marketing to email warm leads, Marketing has no idea who to email.
- Marketing has to go to Engineering for that reporting
- The Sales team could get very different numbers.
- Engineering implements a technical solution, but doesn't consider the Sales process and creates a very manual process. Sales does not use the solution.
- Each regional team has slightly different meanings for each stage

#### Churn:
- people know that churn is bad, and it leads to a decrease of revenue
- when you look at definitions from each org, they end up being completely different
- people are confused.

### Post-Data team

#### The Definitive Data Definition Doc:
- Audited questions, queries, and old emails
- Boiled them down to individual data points
- Came up with names for these data points
    - Wanted to keep as much existing terminology as possible
        - If existing terminology doesn't exist, use standard SaaS def
        - If both don't exist, try to use shared context
- Drew rough diagrams of displayed data at a high level
- Met with stakeholders see if people were confused or surprised, and wanted to break that down
- Want to break down the data to it's desired concept, and have that be understood by stakeholders
- No specific numbers, only talking conceptually
- Once people agree, implement and present some example data and visualizations
    - Goal is to bring abstract concepts into reality and understand data context
- Finalize defintiion and models, put into Data Definitions doc
- Share top level dashboards, and run workshops to introduce new data to folks

## Scaling the process
Scaling engineering is easy, but scaling people is hard
- Stakeholder involvement
    - defining MAU
        - suggested logged in in the past 30 days
        - brought it to people, and folks agreed
            - but were they the right folks? or the folks that the team worked well with
        - sanity check with broader group
            - broader group was not a fan, wanted a more specific definiton
    - make sure you're talking to the right people, but also imo, have sanity checks
- Discoverability
    - Problem: Google doc went from a few pages to 10+
    - Current Solution: 
        - use Google doc for high level things and commonly used words
        - dbt docs for more granular things
            - trying out exposures too
        - write contextual definitions on dashboards 
            - can link back to gdoc or dbt docs
    - really, always be interating, this is a hard problem that isn't solved

## Broad Lessons Learned
- in the end aim for good enough
- if there isn't anyone pushing back on stuff, you might not have the right people selected
- if someone just says good enough, they may be too far from the problem
- they have created a process that is focused on overcoming the three barriers