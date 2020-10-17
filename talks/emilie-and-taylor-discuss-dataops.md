# Emilie and Taylor discuss DataOps
youtube: https://www.youtube.com/watch?v=4SpP3yFiQHI

twitters:
 - [@emilieschario](https://twitter.com/emilieschario)
 - [@tayloramurphy](https://twitter.com/tayloramurphy)

## what is dataops?
three pillars
- driving value to a customer
- decreasing cycle time to analytics
- implementing processes and methodologies with the previous two in mind?

### how does devops compare to dataops?
#### 4 pillars of devops
- faster results
- less things breaking
- security
- keeping customers happy
#### dataops vs devops
- dataops works a lot with managing state
- devops delivers software (or code), dataops delivers inisghts (as a result of code)
#### does the devops figure 8 translate to dataops?
- [wikipedia](https://en.wikipedia.org/wiki/DevOps_toolchain
)
    - dev
        - plan
        - coding
        - building
        - testing
        - packaging
    - ops
        - packaging
        - releasing
        - configuring
        - monitoring
        - plan
- generally, most seem to apply, though it depends on the scope of the team
    - i find releasing and configuring to be the _weakest_ links here, but that is biased by my experience

## how do i get dataops?
- use dbt!
- taylor's talk focused on a technical perspective
    - start with version control and build from there
        - automated jobs
        - environments
        - testing
- the organizational perspective of getting dataops
    - probably determined by the c-suite
        - their execs understand the value data and what getting to a data driven culture mean
    - a lot of conversations with a motivated actor
### what can strong data teams do?
- biz intelligence
    - excellent understanding of the org
    - data team integrates data sources to get a high level and detailed view of the org
        - greenhouse for HR/people
        - netsuite for finance
- product intelligence
    - being able to understand customer pain points
    - test better paths to make the product better
    - product data can help you derive product decisions
#### [data science hierarchy of needs](https://hackernoon.com/the-ai-hierarchy-of-needs-18f111fcc007)
- the top 4 parts of the pyramid fit into data ops: move/store, explore/transform, aggregate/label, learn/optimize
- does collect fit in?
    - it should be
    - they note that the pyramid is all technical, and has no people portion
    - dataops can be whatever you want it to be
    - people in an org are generating a lot of data, and getting insight into that is part of the dataops philosophy
#### reporting, insights, predictions
- emilie's three tiered analysis framework
    - s/o to claire
- can you move into insights without dataops?
    - yes, but in an ad-hoc way
    - we can use the data to move forward without version control and testing, but it won't be reproducible 
    - not everything needs to be repeated, but it should be done in a repeatable way
- repeatability vs scalability
    - scalability
        - people: if your work is repeatable, you can do more work with less people
        - technical: can your code handle terabytes of code
    - they are very related, but you can't have scalability without any source of scalability
        - can't do new things with new people because you're always reinventing the wheel
## can you do dataops with gitlab?
### use meltano!
### gitlab the product
- center your work around issues
    - how can we route all changes through a merge request/pull request
- center your workspace
- center your truth
    - have a handbook that has metric definitions where conversations can be had about "the truth"
#### who needs to use version control?
- everybody should understand high level concepts of version control, but not the low level stuff
- not everything needs to be version controlled
## the taylor murphy plan to implement dataops in your data team (patent pending)
1. take a step back
    - think about what you're trying to do as a team
    - where do you want to go? where do you want to go next?
2. going to need to invest in things
    - tools $$
        - data warehouse
        - stitch/fivetran
    - people $$$
3. start thinking about the processes that you're defining in the work that you do
    - document it
    - become operationally mature
4. how can i do things in the concept of a merge request
5. technical things
    - automate things
    - test things
    - scale things
