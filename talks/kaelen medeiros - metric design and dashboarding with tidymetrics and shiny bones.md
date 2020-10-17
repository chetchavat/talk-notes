# Kaelen Medeiros - Metric Design and Dashboarding with tidymetrics and shinybones

Link: https://www.youtube.com/watch?v=BL5NBRxnl3E

## North Star Metrics (NSM)
- one metric that measures how your product delivers value to its users
- NSMs should be something that drive retention, and a proxy for revenue 
    - airbnb: nights booked
    - facebook: # users adding 7 friends in 10 days
        - evolved from DAU
        - heyo this one again
    - duolingo: daily active users
- NSMs can easily be gamed
    - such as buying low quality views/clicks/users
        - low LTV leads
- "when a metric becomes a target, it ceases to become a good measure" - marilyn strathern, summariing Goodhart's law

### Safety "metrics"
- the yin to NSM's yang
- metrics that guard against gaming, artificial inflations etc.
- provides a system to think hard about what success really means

metric design on the stack overflow R questions dataset
- NSM
    - \# questions asked = avg # questions asked * # active users
    - avg # of questions = # questions asked / # active users
    - \# active users = # users * % users active
- NSM decomposes into 5 different metrics
    - \# of users
    - \# of questions
    - \# active users
    - % active users
    - avg # of questions asked by active users
## tidy metrics
wow time for some R magic?

tidymetrics creates metrics in a tidy way

### cross_by_period
- Cross by any set of calendar periods (like day or week), rolling windows, or recent intervals (like "4 Weeks", or "8 Weeks"). 
- This means that each row in the input will appear potentially multiple times, each time associated with a different period and date.
    - requires a date formatted column named date
    - creates summarized output across provided date intervals
### cross_by_dimensions
- acts as an extended group_by that allows complete summaries across each individual dimension and possible combinations.
    - accepts a categorical and crosses every possible combo of dimensions and periods before calculating an outcome

R really is magic
- `use_metrics_scaffold()`

shiny is also magic