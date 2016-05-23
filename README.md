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

1. U.S. - whooping cough, rabies, salmonellosis and E. coli Infection. Time
   period of study: January 2010 to December 2013. Evaluation period for
   disease incidence estimation- January 2012 to December 2013. Official disease case counts
   obtained from Project Tycho (https://www.tycho.pitt.edu/).

2. China - H7N9, HFMD and dengue. Time period of study: January 2013 to
   December 2014. Evaluation period for
   disease incidence estimation- December 2013 to December 2014. OOfficial disease case counts obtained from National Health
   and Family Planning Commission (http://en.nhfpc.gov.cn/).

3. India - acute diarrheal disease (ADD), dengue, malaria. Time period of
   study: January 2013 to December 2014. Evaluation period for
   disease incidence estimation- April 2013 to December 2014. Official disease case counts obtained
   from Integrated Disease Surveillance Programme (http://www.idsp.nic.in/).

Raw HealthMap data

We obtained a corpus of disease-related news articles from HealthMap for each of the 3
countries - U.S., China and India. The corpus contains articles related to the
diseases of interest for each country. The raw HealthMap corpus corresponding
to U.S., China and India can be found in
https://github.com/sauravcsvt/EpiNews_supplementary_data/tree/master/data/US/raw_HealthMap,
https://github.com/sauravcsvt/EpiNews_supplementary_data/tree/master/data/China/raw_HealthMap and
https://github.com/sauravcsvt/EpiNews_supplementary_data/tree/master/data/India/raw_HealthMap.
