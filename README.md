# EpiNews_supplementary_data

Supplementary dataset associated with the manuscript 'Temporal Topic
Modeling to Assess Associations between News Trends and Infectious Disease
Outbreaks'. In this manuscript, we introduce 'EpiNews', a generic
temporal framework that combines supervised temporal topic models with
time-series regression techniques to monitor and estimate time-varying
incidence of multiple diseases. We validated 'EpiNews' against official 
disease case count reports, as available from public healh agencies, in U.S.,
China and India. We evaluated 'EpiNews' on multiple 
disease outbreaks in the recent past, such as whooping cough in U.S. (2012),
periodic outbreaks of avian influenza A (H7N9) and hand, foot, and mouth disease (HFMD) 
in China (2013 and 2014), dengue outbreaks in China (2014) and India (2013). Given below 
are the diseases for which we evaluated 'EpiNews' for U.S., China and India.

* U.S. - whooping cough, rabies, salmonellosis and E. coli Infection. Time
   period of study: January 2010 to December 2013. Evaluation period for
   disease incidence estimation- January 2012 to December 2013. Official disease case counts
   obtained from Project Tycho (https://www.tycho.pitt.edu/).

* China - H7N9, HFMD and dengue. Time period of study: January 2013 to
   December 2014. Evaluation period for
   disease incidence estimation- December 2013 to December 2014. Official disease case counts obtained from National Health
   and Family Planning Commission (http://en.nhfpc.gov.cn/).

* India - acute diarrheal disease (ADD), dengue, malaria. Time period of
   study: January 2013 to December 2014. Evaluation period for
   disease incidence estimation- April 2013 to December 2014. Official disease case counts obtained
   from Integrated Disease Surveillance Programme (http://www.idsp.nic.in/).

## Raw HealthMap data

We obtained a corpus of disease-related news articles from HealthMap for each of the 3
countries - U.S., China and India. For each country, the corpus contains articles related to the
diseases mentioned above.

* [Raw HealthMap U.S.](./data/US/raw_HealthMap/)
* [Raw HealthMap China](./data/China/raw_HealthMap/)
* [Raw HealthMap India](./data/India/raw_HealthMap/)

## Processed HealthMap data

The corpus for each country was preprocessed and transformed to a collection of
tuples of the form {w,l,t}: count where count is the number of news articles
mentioning the word w referring to location l at time point t. For each
country, the sets of such tuples were provided corresponding to each time point T within the
evaluation period. E.g., for China, the file 'tuple collection-2014-02-01.csv' contains the
set of tuples from t=0 ('2013-01-01') to t=T where T='2014-02-01'.
T='2014-02-01' refers to the month of February 2014. The tuple "('h7n9',
('China', u'Shandong'), '2013-04-01')",1 means that the word 'h7n9' was
mentioned in 1 article referring to the province of Shandong in China over the
month of April 2013. Similar definition applies to the set of tuple collections
obtained for U.S. and India except the fact that each time point t represents a
period of 1 week.

* [Processed HealthMap U.S.](./data/US/processed_HealthMap/)
* [Processed HealthMap China](./data/China/processed_HealthMap/)
* [Processed HealthMap India](./data/India/processed_HealthMap/)



## Topic Distributions

The first component of 'EpiNews' is a supervised topic model which extracts
latent disease topics and their associated temporal trends of prominence from
the set of tuple collections. The temporal topic trends (along with the sampled 
case counts generated via multinomial sampling) for the diseases were provided 
corresponding to each time point T within the evaluation period. 

* [Topic distributions U.S.](./data/US/topic_distributions/)
* [Topic distributions China](./data/China/topic_distributions/)
* [Topic distributions India](./data/India/topic_distributions/)



