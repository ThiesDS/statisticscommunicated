+++
# Custom widget.
# An example of using the custom widget to create your own homepage section.
# To create more sections, duplicate this file and edit the values below as desired.
widget = "custom"
active = true
date = 2016-04-20T00:00:00

# Note: a full width section format can be enabled by commenting out the `title` and `subtitle` with a `#`.
title = "Data Science Toolbox"
subtitle = ""

# Order that this section will appear in.
weight = 2

+++

## Statistics Analysis

For statistical analysis and visualization I really like to use R. Especially the [tidyverse](https://www.tidyverse.org/) packages like [dplyr](https://www.rdocumentation.org/packages/dplyr) and [ggplot2](https://www.rdocumentation.org/packages/ggplot2) allow for an intuitive workflow and great-looking, publishable figures that lets quickly explore every dataset. When it comes to reporting I write static reports in [rmarkdown](https://rmarkdown.rstudio.com/) as it enables reproducable work. Beyond that I'm a big fan of interactive [shiny](https://shiny.rstudio.com/) applications. Especially extending shiny with the [shinydashboard](https://rstudio.github.io/shinydashboard/index.html) package enables great-looking web apps out of the box. Actually, in our organization we don't only use shiny as reporting tool but use them in production. 

## Model Building

When it comes to model building I like to think about problems from either a machine learning or a statistical perspective. When I simply need to predict something, I use traditional machine learning models trained with [caret](https://topepo.github.io/caret/index.html) when it is feasable on my local machine. If this is not possible I mainly go back to utilize [h2o](https://www.h2o.ai/) for distributed computing of heavy-weight machine learning tasks. Once the models are trained, I mostly use [LIME](https://cran.r-project.org/web/packages/lime/vignettes/Understanding_lime.html) (short for *Local Interpretable Model-Agnostic Explanations*) to give me an understanding of why these predictions occured. However, if the main goal is to really understand how certain things in the world work, I like to build bayesian models using pythons probabilistic programming library [pymc3](https://docs.pymc.io/). There is a great talk called [Machine Learning and Statistics: 
Don't mind the gap](https://docs.google.com/presentation/d/1buknIrG5b8u0twrwvlxcTudIOdx68AlqDiST_A_jJ9g/edit#slide=id.p) by [Thomas Wiecky](https://twitter.com/twiecki) that addresses to bridge the existing gap between machine learning and statistics.

## Workflow Management & Deployment

Apart from the core tools, I use [git](https://git-scm.com/) for version control and collaborative development and [docker](https://www.docker.com/) for deployment of e.g. shiny applications.

Currently I'm testing [apache airflow](https://airflow.apache.org/) as it is a great tool to manage ETL processes for a data warehouse and it seems to be fairly easy to manage your machine learning pipeline with it. 