
# Natural Disasters: Analyzing Worldwide Risk Perception & Experience
> This project utilized survey data from the Lloyds Register Foundation World Risk Poll and the EM-DAT International Disaster Database to explore the correlation between perception of risk from natural disasters and actual experience of natural disasters. I also analyzed factors such as country-level experience, disaster severity, and differences in risk perception based on demographic differences.


## Table of Contents
* [Motivation](#motivation)
* [Data Sources](#data-sources)
* [Data Questions](#data-questions)
* [Cleaning and Analysis Process](#cleaning-and-analysis)
* [Further Recommendations](#recommendations)
* [Contact](#contact)



## Motivation
I grew up in Kansas, within what is called “Tornado Alley”, where tornado watches and warnings were a common occurrence during the spring & summer months. My town was never directly hit, although I remember in high school going to a nearby town to volunteer with cleanup efforts for a town that was nearly destroyed. Perhaps because I was never directly affected, I never felt afraid of tornadoes. 

Since I moved to Nashville in 2009, we have experienced a “1000-year flood”, 2 tornadoes, a derecho, and many smaller storms. Seeing the impact of the 2020 tornado especially on my friends, neighbors, and beloved neighborhood businesses gave me a much greater fear and respect for tornadoes, and I now am very cautious when there is risk of severe storms and tornadoes. 

These personal experiences led me to an interest in exploring the impact of all types of natural disasters on people’s feelings of risk, and especially the effect of personal experiences of living through a disaster. My background in social work drives my interest in mental health and anxiety connected with these disasters. Also, given the increasing occurrence of extreme weather events due to climate change, this topic will be a growing area for concern.


## Data Sources
I used 2 data sets for this project - both are readily available to the public online. 

- The Lloyds Register Foundation World Risk Poll - https://wrp.lrfoundation.org.uk/world-risk-poll-data
The Lloyds Register Foundation is an independent global charity based in London. 
Their World Risk survey was conducted in 2019, 2021, and 2023 to assess feelings of risk from a variety of different topics among people around the world. 
For this project I utilized their 2021 dataset which surveyed almost 126,000 people in 121 countries. One limitation of the data I noticed is that Africa is underrepresented in the country list - a lot of countries in Africa were not surveyed.
More information on survey methodology can be found in the methodology PDF above.

- EM-DAT: The International Disaster Database - https://public.emdat.be/
This database is maintained by the Centre for Research on the Epidemiology of Disasters, based at the University of Louvain in Brussels, Belgium. Their database contains information on disasters around the world between 1900 and the present; it is regularly being updated as new disasters occur. 
  

## Data Questions
- Does having personal experience of a natural disaster impact your perception of risk from natural disasters? 
- How do demographic factors impact perception of risk from natural disasters? 
- Is there a relationship between perception of risk from natural disasters and country-level experience? 
- Is risk perception correlated with disaster severity?


## Cleaning and Analysis Process
1. I began with cleaning the World Risk Survey data. The original dataset had 243 columns; I dropped the columns related to risk categories not dealing with natural disasters, as well as columns related to regions for each country in the survey. I had originally hoped to identify disaster-affected areas by region, but quickly realized that the regions/locations specified in the survey dataset did not match up with ones in the disasters dataset. Therefore, the location analysis in this project is based on countries as a whole.

One challenge with this dataset was that the answers to each survey question and demographic marker for each participant were coded as numbers. In Python, I created a data dictionary for each coded column (50 in total) and remapped the values so that each participant's answer was listed rather than just a number. 

I also dropped rows related to the 2019 survey responses. With more time, I would have liked to analyze the difference in responses between 2019 and 2021, and compare to disasters that occurred between the 2 surveys.

2. The EM-DAT data didn't require as much intensive cleaning. I removed all disasters classified as "Technological" and "Biological" since my focus was on natural disasters. More information on disaster classification can be found here: https://doc.emdat.be/docs/data-structure-and-content/disaster-classification-system/

As I continued my analysis, I also created a subset of the disaster dataset looking at just the five-year period prior to the survey being administered. I used this for most of my analysis, as one of the survey questions asked about experience with disasters in the last five years. 

3. One of the main challenges in analysis was the abundance of data in both datasets, and deciding which measures would be most appropriate to answer the data questions I had set for myself. As I explored the data I gradually determined which columns in the datasets would be best to measure what I was looking for - these are further explained in the dashboard and accompanying video.

As I looked at how different factors influenced risk perception, I was able to use tools such as slicers and key influencer graphics in my Power BI dashboard to illuminate the impact of those factors. I also used color in bar charts and maps to highlight commonalities between the two datasets.

## Further Recommendations
As I thought about the impact of my analysis and my recommendations for next steps, I focused on the idea of disaster preparedness. Obviously we can't prevent natural disasters from happening, but we can empower people with the tools to be prepared. My social work background led me to curiosity about the best ways to do that, and how to incorporate mental health support into that preparedness work. As mentioned on the last tab of the dashboard, I found a study done in 2020 in Haiti in an earthquake and flood-prone area. Through an intervention conducted by native Haitians, participants were able to receive information about how to prepare as well as how to maintain their mental health. Significant results were achieved through this work, and I hope something like it can be expanded to other places like Southeast Asia, which experiences frequent and severe disasters.   

##Contact
Please reach out via email at eem.chadwick@gmail.com with any questions! 

-Emily Chadwick


