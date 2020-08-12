# Marlorie Hughes - Dashboarding Like a Boss
Link: https://www.youtube.com/watch?v=yott4quKN6s

her slides are in a dashboard!
- https://maloriejhughes.github.io/Dashboarding-Tutorial/
## "i create dashboards at the end of every analysis" why bother? 
- dashboards are organized
    - don't email a picture or a csv, it'll get lost
    - keeps things organized and pretty
- dashboarding is a low risk, exploratory, learning process
    - since you're just organizing your plots you can take templates and see what works
    - go to marlorie's github to steal dashboard templates
- dashboards have better visualizations
    - interactivity
    - she is referring to a very specific version of a dashboard, but nowadays most dashboards are relatively interactive (thanks BI)
- dashboards are flexible and reproducible

## a 12 step program to quit emailing plots and csvs
1. basic layout
    - this talk uses flexdashboard
    - i should look into flexdashboard
1. printing
    - tables, descriptive stas, model summaries
    - `print()` is not okay, we want to make pretty things
        - `printr`
            - overwrites base `head()` and `summary()`
        - also `knitr::kable`
            requires you to change you base code
        - `summarytools`
            - could theoretically have plots of distributions right now
        - for model summary, user `stargazer`, looks like latex
1. interactive datasets
    - printing tables vs `DT::datatable()`
        - `DT::datatable()` is pretty and interactive!
1. interactive plots 
    - highcharter
    - go to her github for more details
    - other viz
        - maps: leaflet
        - timeseries: dygraphs
        - ggplot2 compatible: plotly
1. exporting
1. css basics
    - copy someone else's css
1. branding
    - logos, font, colors
1. header/footer
1. hosting
    - wanna do it internally, find a sysadmin
1. automate-ish
    - render + system()
1. replicate
    - render with arguments
1. automate it or app it
    - cron, shiny runtime
    - turning flexdashboards into shiny is easy

## making dashboards pretty is important
- pretty is important.

## protips
- simple
    - start with a simple template and someone elses css
    - add in essentials or the lowest hanging fruit as you go
- organized
    - maintain a folder containing
        - css, exporting scripts, color pallettes, global themes, and templates
    - keep a staging foler for exploration
        - don't make changes you won't know how to undo
- explore
    - try something new to improve the usability of each new dashboard
        - templates, plots, css
    - slowly work in
        - about page and explanations
        - interactivity
        - exporting
        - logos
        - footer
        - padding or margins
