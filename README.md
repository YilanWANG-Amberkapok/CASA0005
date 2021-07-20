# Instructions

## Submission

On clicking the exam link a new repository has been created for you in the exam classroom. You should now clone this repository into a new RStudio project then **knit, commit and push** to GitHub as usual. 

You must knit your final `exam_response.Rmd` to `html` and ensure you push to GitHub before the deadline.

GitHub takes a snapshot of your **local git** repository at the deadline so **knit, commit and push often**, as you should do in all spatial data science projects. The deadline is based on your last commit, but we expect the repository to be pushed to GitHub very soon after. 

## Before you begin: 

* Go to the top of the `exam_response.Rmd` RMarkdown document and edit the name and student number fields (at the top of the `.Rmd`).

* Complete the originality declaration

## Task

You have four hours to complete this open book exam. You must select and undertake **only one** of the research questions below. Data for each question has been provided in the relevant folder and you are free to source additional data for extension analysis but everything you need is provided.

* You must write your response in the `exam_response.Rmd`, under the originality declaration.

* You may use any resource to assist you but the work must be your own and you are required to sign a originality statement within the exam. 

* Questions about the exam must be asked on the open Slack GIS channel. 

* You can use RStudio visual markdown editor if you wish.

* If you copy section of code from an online source please provide a relevant link or acknowledgment.

Marks are awarded as per the marking scheme. It's important to note there is no 'right' answer, even if your findings are inconclusive or not as expected, you are awarded marks for how you approach the problem.  

## Within your work you must:

* Provide an initial project scope in bullet point form, detailing the process and data wangling and analysis you intend to undertake, prior to starting the analysis. 

* Produce a well commented and fully explained RMarkdown document that attempts to answer the research question.

* Create at least one graphical output and at least one mapped output.

## Tips:

* You are able to propose a variation of the original question (e.g. selecting a specific year of data to analyse) based on appropriate reasoning, but this must be clearly stated. 

* Expectations of the assignment are relative to the time allocated. Do not waste time trying to propose / develop the most advanced or innovative form of analysis.

* Do the basis well. 

* Structure your RMarkdown document with titles and subtitles. 

* Comment and explain your working throughout.

* State assumptions and describe limitations.

* In most questions some administrative boundary data has been provided, use this to assist guiding recommendations and outputs.

# Practice Question

## New York Evictions

New York City wish to conduct a study that aims to prevent people being evicted by understand possible related factors. They have appointed you as a contractor to determine if there was a spatial pattern in evictions in 2020.  

### Data

* List of evictions
* New York City community districts 

## The impacts of redlining on social equity  

Starting in the 1930s the American Home Owners' Loan Corporation (HOLC) was tasked with refinancing mortgages on properties to prevent missed payments. To do this the HOLC assessed the "credit-worthiness" of neighbourhoods, dividing them largely on race into grades between A, considered the "best", and D considered "hazardous", drawn around in red, hence the term "redlining". Other services such as healthcare and infrastructure investments were decided in similar way. 

The Civil Rights Act of 1968 (the Fair Housing Act) made it unlawful to discriminate housing or financing in this manner. However, the redlining legacy has left severe social equity issues across cities, such as access to outdoor space, clean air and trees. 

Vegetation has a large impact on local temperature,  with heat being the leading cause of weather related deaths in the USA. You have been tasked to establish to what extent current temperature differs across the HOLC "graded neighbourhoods" in Los Angeles.  

### Data

* Los Angeles redlining shapefile
* Landsat surface reflectance image
* Los Angeles census tracts (outline of which is the city of Los Angeles)

## Graffiti mitigation 

In 2004 the city of San Francisco stopped cleaning graffiti on private property passing the responsibility to property owners who must act within 30 days or face a $500 fine. A local group of business owners are getting frustrated by the cost of continually removing graffiti. They have appointed you to identify factors that might geographically influence graffiti occurrence so they can present a case to the city for pro-active measures.

### Data

* Household data (census tract)
* Education data (census tract)
* Household income data (numbers on households in each category) (census tract)
* Population age data (census tract)
* Household income in dollars (census tract)
* Poverty status (census tract)
* Private Health insurance coverage (census tract)
* Census tract spatial data
* Graffiti points
