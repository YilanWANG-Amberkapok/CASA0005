# Instructions

## Submission

On clicking the exam link a new repository has been created for you in the exam classroom. You should now clone this repository into a new RStudio project then commit and push to GitHub as usual. Remember that your repository must appear in the GitHub classroom platform. Do not clone the repository to a location outside the GitHub classroom as this will not be marked.

GitHub takes a snapshot of your local git repository at the deadline so commit and push often (e.g. once per hour), as you should do in all spatial data science projects. The deadline is based on your last commit, but we expect the repository to be pushed to GitHub very soon after.


## Before you begin: 

* Go to the top of the `exam_response.Rmd` RMarkdown document and edit the name and student number fields (at the top of the .Rmd).

* Complete the originality declaration


## Task

You have six hours to complete this open book exam. You must select and undertake only one of the research questions below. Links to the data for each question have been provided and you are free to source additional data for extension analysis, but everything you need is provided.

* You must write your response in the exam_response.Rmd, under the originality declaration.

* You may use any resource to assist you but the work must be your own and you are required to sign an originality statement within the exam. Clearly acknowledge and state if/where AI has been used.

* Questions about the exam must be asked on the open Slack GIS channel.

* If you copy a section of code from an online source please provide a relevant link or acknowledgment.

Marks are awarded as per the marking scheme. It's important to note there is no 'right' answer, even if your findings are inconclusive or not as expected, you are awarded marks for how you approach the problem.

## Within your work you must:

* Provide an initial project scope in bullet point form. Your project scope should include:

  * If you intend to propose a variation of the original question (e.g. selecting a specific year of data to analyse), this must be based on appropriate reasoning and clearly stated.
  * A brief background to the topic.
  * A research question and/or hypothesis.
  * An evaluation of your research datasets.
  * An explanation of additional data that you might have sourced for your analysis (it is not a requirement to source additional data).
  * An explanation of the data wrangling you intend to undertake.
  * A justified plan for the spatial data analysis that will be required.
  * You may also wish to identify any constraints around the data you have been instructed to analyse or obvious omissions from the set task that could limit what will be produced in this short project. These could relate to spatial or temporal limitations in the dataset, what you decide is reasonable to analyse or anything else that is relevant.


* Commit and push regularly (e.g. once per hour) during the final exam.

* Provide any data your have sourced, unless it exceeds the GitHub upload limit, in which case a URL that links directly to the exact dataset must be given.

* Produce a well commented and fully explained RMarkdown document that attempts to answer the research question.

* Create at least one graphical output and at least one mapped output.

* Critically reflect on the results you have produced.

## Tips:

* In the time you have, prioritise good solid analysis tailored to answering your research question over elaborate approaches that produce lots of results that don’t directly contribute to answering your research question. 

* Structure your RMarkdown document with titles and subtitles.

* Comment and explain your working throughout.

* State assumptions and describe limitations.

* In most questions some administrative boundary data has been provided, use this to assist guiding recommendations and outputs.

* Provide critical commentary about the data you are using and the analysis you are undertaking throughout.

* Plan your time. We suggest 1 hour for data exploration, 2-3 hours for analysis, 1 hour for visualisations, 1 hour for interpretation and reflection. 

# Practice Question

## New York Evictions

New York City wish to conduct a study that aims to prevent people being evicted through understand possible related factors.You have been enlisted as a consultant and tasked to conduct an analysis of their data from 2020.

You should use appropriate data processing and analysis methods to produce an overview report which summarises the patterns revealed in the data in this year. It is expected that at least some of the methods you use will relate to the spatial dimensions of the data.

Your report should include a brief introduction including relevant contextual information at the beginning and a critical review of your findings at the end. You must include at least one map. 

### Data

* List of evictions - https://data.cityofnewyork.us/City-Government/Evictions/6z8x-wfk4
* New York City community districts - https://www.nyc.gov/content/planning/pages/resources/datasets/community-districts

## Graffiti mitigation 

In 2004 the city of San Francisco stopped cleaning graffiti on private property passing the responsibility to property owners who must act within 30 days or face a $500 fine. A local group of business owners are getting frustrated by the cost of continually removing graffiti. 

The local business owners have enlisted you as a consultant and tasked you to conduct an analysis of possible contributing factors to graffiti occurrence so they can present a case to city legislators for pro-active measures. 

You should use appropriate data processing and analysis methods to produce an overview report which summarises the patterns revealed in the data. It is expected that at least some of the methods you use will relate to the spatial dimensions of the data.

Your report should include a brief introduction including relevant contextual information at the beginning and a critical review of your findings at the end. You must include at least one map.

### Data

* Census tract spatial data - https://www.census.gov/cgi-bin/geo/shapefiles/

* Graffiti points - https://data.sfgov.org/City-Infrastructure/Graffiti/vg6y-3pcr 

* American Community Household Survey: https://data.census.gov/cedsci/advanced

Under Geographies: Census Tract > California > All Census Tracts within California > tables > then you can filter on a keyword and download tables.

From the American Community Household Survey you might consider using:

  * Age and Sex (census tract)
  * Educational Attainment (census tract)
  * Households and Families (census tract)
  * Income in the Past 12 Months (numbers on households in each category) (census tract)
  * Poverty Status in the Past 12 Months (census tract)
  * Selected Characteristics of Health Insurance (census tract)
  
