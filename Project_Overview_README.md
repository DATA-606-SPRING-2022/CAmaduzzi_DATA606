# NOTE: A full report delineating the project process and findings can be read in the folder titled Final Project Documents 
# Here you will find all of the final documents relating to the Capstone Project overall.



# CAmaduzzi_DATA606
## Data 606 Capstone Project


## Introduction
Access to education has always been considered one of the most important factors that can lead to more equitable and just social structures within societies. Higher education in particular is considered to be an essential mean through which to open greater opportunities for professional, and consequently financial, success, ultimately leading to greater social mobility and thus greater fairness for all members of the population. In other words, admissions into Higher Education institutions, and ultimately enrollment, can open the door to productive and meaningful futures, even when taking into consideration reduced social mobility. 
 
Higher Education Institutions (HEI) are, for all practical purposes, rather large organizations that have significant impact on the economies of the States they are located in (and beyond) – both directly (via the jobs and contracts they create) and indirectly (thanks to the professional work-force they contribute to). They are organizations that need to remain healthy and productive for the long term growth and health of our society. 
 
In recent years, HEI have been reporting a decline in enrollment. Publicly available information seems to confirm this trend, in particular for undergraduate programs. (NSCRC, 2021)
 
Given the wide impact HEI have on the long term growth potential of a Community, a State, and more broadly of the Nation, it is important to understand the factors that influence students towards enrollment in HEI. Using only publicly available information reported by HEI themselves, I intend to take a closer look at these features under HEI’s direct control to try to identify those having the greatest impact on students’ undergraduate enrollment and possibly open avenues for further research and/or interventions for HEI to test. 


## Research Questions
The questions I am interested in looking into are the following:  
1)	Based on publicly reported information regarding HEIs, what features seem to affect student enrollment choice the most? 
2)	With an eye to I.D.E.A. (Inclusion, Diversity, Equity, and Access), do HEIs with different structural characteristics, fare differently across the US?
3)	Are new policies adopted by HEIs, such as standardized-tests-blind admission policies, having an effect on students’ enrollment? 


## Data
One of the primary difficulties in working with education data is that most of the data that is openly accessible is observational in nature. In addition, when, and if, any randomized control trials are conducted, sample sizes are relatively small and usually not publicly available. Furthermore, education data acquires greater meaning when analyzed over a certain period of time, a certain number of years. In fact, this type of analysis allows to uncover trends or changes over time that would otherwise not be immediate. 
 
Recent research studies have suggested however, that using auxiliary observational data (sometimes referred to as remnant data, ie data that did not get used in a randomized control trial) in conjunction with machine learning techniques, can actually successfully enhance/improve the conclusions reached through a randomized trial, without negatively affecting bias, precision, or introducing additional assumptions) (Gagnon-Bartsch et al. 2021) This result, as pointed out by the researchers themselves, has tremendous potential for research in education where the characteristic of having access to large observational datasets is the norm, and not the exception. 
 
If these initial research results will be confirmed, greater reliability will be given to the results of this research initiative as well. In fact, for this project the data used is publicly available structured data from IPDES (The Integrated Postsecondary Education Data System) which is a centralized data repository made available through the National Center for Education Statistics (NCES) (https://nces.ed.gov/ipeds/ and https://nces.ed.gov/ipeds/use-the-data ), which is collected via direct reporting by the HEIs themselves, sometimes begrudgingly. 
 
HEIs report to IPDES by completing mandatory surveys. These reporting requirements are the direct result of the HEIs participation in Federally funded programs authorized via the Higher Education Act of 1965 (Title IV), the Civil Rights’ Act of 1964 (Title VI), and/or the Education Amendments of 1972 (Title IX), and later amendments. When not compliant, HEIs can be fined and suffer further consequences. 
 
The existence of this data is particularly interesting, given the fact that it has been collected over time and thus can given us an instrument to highlight the changes occurring in HEIs enrollments over time. 


## Project & Data Focus
The project, on the one hand side, describes the data selected to highlight existing similarities in terms of enrollment and organizational structure across HEIs over time; on the other hand side, uses machine learning techniques to verify the existence of these similarities and highlight the most significant publicly available features that emerge as primary drivers of student enrollment. 
 
To make the analysis mostly reliable, the data utilized will only include data reported directly by the HEIs and it will focus on a few selected years, conveniently spread apart (probably about 5 years apart). Geographically focus will be placed on the State of Maryland Institutions – but this may be extended based on initial results, if necessary. 
 
The IPDES data sets available are relatively broad and provide a lot of different information regarding HEIs and their student admission and enrollment characteristics. 
 
Here is an initial (and non-exhaustive) list of variables that will be selected by area of topic:
### -	Institution identification and characteristics information 
- Unique ID number
- State
- HBCU status
- Locality (rural vs urban etc) 
- Primary post-secondary focus 
- Open admission Policy 
- Accepting AP course credit
- ROTC program offering
- Student support services 
- Tuition support plans
- Room and Board charges
- Tuition costs
- Additional Fees  
- Faculty
 
### -	Student Admissions and Enrollment data
- Admissions by race and gender
- Enrollments by raceand gender
- Secondary school average GPA, rank and record 
- SAT and/or ACT scores  
 
All of the variable choices are spread across various data sheets publicly available and can be found here: https://nces.ed.gov/ipeds/datacenter/DataFiles.aspx?gotoReportId=7&fromIpeds=true 


## ML Algorithms and Analysis 
Given the two-tiered approach I am expecting to acquire greater clarity on the research process and the selection of the most appropriate Machine Learning (ML) algorithms through initial data exploration. 
 
Some traditional aggregative models and data description tools will be used to visualize common characteristics among HEIs and then determine how to best subdivide the organizations. 
 
Based on this a priori analysis and segmentation, which could be confirmed or evaluated by using a ML clustering algorithm (such as DBSCAN, which is nonparametric), I will then analyze the effect of the selected features to start answering the research questions asked. 
 
I plan to approach the identification of the most significant features using a couple of algorithms. I would probably like to use a feature importance extraction technique such as a PCA (Principal Component Analysis) unsupervised approach to identify the primary features affecting undergraduate enrollment and then use a regression model to confirm predictive accuracy. 
 
The data being used is structured data, mostly quantitative, but it also includes some categorical elements which will require to be handled appropriately.
Lazypredict will be used as a way to help verify the appropriateness of the model selection process.
If possible, I would also like to further the analysis by finding ways to highlight and model the institutions based on their Inclusion, Diversity, Equity, and Access (I.D.E.A.) variables/variable-scores.  
 
If I verify the existence of significant differences in enrollment predictions, I plan to try to identify modeling approaches that may explain and/or support the differences. 
Tool-wise, I may choose to use Databricks Community edition to handle the aggregated data more efficiently, especially if I extend the analysis beyond the single State of Maryland. 


## In Conclusion
I am hopeful that the project will show some interesting data regarding student enrollment which tends to be overlooked by researchers. 
Basing the work only on publicly available information I am hopeful to contribute to the discussion in the field of higher education, especially in connection to the challenges involving Inclusion, Diversity, Equity and Accessibility, while leaving ample room for further analysis. I am hopeful that interesting findings will emerge. 
 
 
## References: 
- National Student Research Clearinghouse Research Center (NSCRC) https://nscresearchcenter.org/stay-informed/
- Gagnon-Bartsch J.A., Sales A.C., Wu E., Botelho A. F., Erickson J.A., Miratrix L.W., Heffernan N.T. (Submitted on 7 May 2021), Precise Unbiased Estimation in Randomized Experiments using Auxiliary Observational Data, Cornell University.  https://arxiv.org/abs/2105.03529 


