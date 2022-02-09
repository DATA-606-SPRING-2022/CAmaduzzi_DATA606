# CAmaduzzi_DATA606
Data 606 Capstone Project

## 1.	What is your issue of interest (provide sufficient background information)?
Throughout the classes I have taken at UMBC while enrolled in the Data Science program I have continued to analyze themes related to education – from an overview of the national education system at the K-12 level to a more focused analysis of the NY educational system where looked at its composition and whether school location affected school district characteristics, from an analysis of the Higher Education enrollment race interrelations across the US (for purely hypothetical and educational purposes), to, together with a peer-student group, the effects of various different school characteristics on High School graduation rates.
One of the primary difficulties in working with education data is that most of the data that is openly accessible is observational in nature. When, and if, any randomized control trials are conducted, the sample sizes of the data are relatively small and usually not publicly available. – Recent research studies have suggested however, that using observational data (referred to as remnant data, ie data that did not emerge from a randomized control trial) in conjunction with machine learning techniques, can actually successfully enhance/improve the conclusions reached through the randomized trial, without negatively affecting bias, precision, or introducing additional assumptions) (Gagnon-Bartsch et al. 2021) 
Furthermore, education data acquires greater meaning when analyzed over a certain period of time, a certain number of years. In fact, this type of analysis allows to uncover trends or changes over time that would otherwise not be clear. 
For this research proposal I would like to continue to pursue my understanding and analysis of education and its ramifications. In particular I would like to higher education institutions’ enrollment data and analyze the elements that may contribute in undergraduate students’ enrollment, based on publicly available information.

## 2.	Why is this issue important to you and/or to others?
Access to education has always been considered one of the most important factors that can lead to a more equitable and just social structures within societies. Higher education in particular is considered to be an essential mean through which to open greater opportunities for professional, and consequently financial, success for people, ultimately leading to greater social mobility and thus greater fairness for all members of the population. 

## 3.	What questions do you have in mind and would like to answer?
The questions I am interested in looking into are the following:  
1)	What among the publicly available data attributes seem to affect student enrollment choice in higher education Institutions? Does the data seem to confirm a decline in higher level enrollment over these past years and is this true across student groups (as identified by race) or not? 
2)	What models leveraging on the identified features seem to influence enrollment the most? 
3)	With an eye to I.D.E.A. (Inclusion, Diversity, Equity, and Access), do institutions fare differently across the US? Is data publicly available to discern between these three aspects or not? If, not, are there proxies that could be identified instead?

## 4.	Where do you get the data to analyze and help answer your questions (creditability of source, quality of data, size of data, attributes of data. etc.)?
The data I intend to use is publicly available structured data from IPDES (The Integrated Postsecondary Education Data System) which is a centralized data repository made available through the National Center for Education Statistics (NCES) which is administered by the Education Department through Ed.gov (https://nces.ed.gov/ipeds/ and https://nces.ed.gov/ipeds/use-the-data )

## 5.	What will be your unit of analysis (for example, patient, organization, or country)? Roughly how many units (observations) do you expect to analyze?
I will focus my analysis on Higher Education institutions in the State of Maryland, however, if I realize that the data would be most significant if extended to the Nation, then I will expand the analysis to include all States (or maybe a subgroup for example only States in the East portion of the US). 

## 6.	What variables/measures do you plan to use in your analysis (variables should be tied to the questions in #3)?
The data sets available are relatively broad and provide a lot of different higher education institutions information. 
The data I intend to select will include data inherent to the identification of the institutions; its undergraduate student body composition; graduation rates; faculty; cost; location; and admissions. 
I need a little more time to focus my variable choices since the data sources are spread across various data sheets. All can be found here: https://nces.ed.gov/ipeds/datacenter/DataFiles.aspx?gotoReportId=7&fromIpeds=true 
Note: I have used this data in a prior research project, thus I am aware of the fact that the data has some limitations. Primarily, some data is not reported by the institutions directly, but rather derived in some form. I will restrict use to only directly reported data. 

## 7.	What kinds of techniques/models do you plan to use (for example, clustering, NLP, ARIMA, etc.)?
I have to admit that I have not gotten this far in my initial draft proposal, however, I am expecting to aid in the identification of  most significant features via a feature selection model to minimize or at least reduce the number of variables/attributes analyzed. The data being used is structured data, mostly quantitative, but it also includes some categorical elements which will require to be handled appropriately.
I expect to use Lazypredict as a way to help in the model selection process. I suspect that I will apply a regression model to evaluate the variables’ effectiveness in predicting students’ enrollment, and a classification model as well, however, I have not yet clarified my thoughts this far. If possible, I would also like to consider using an unsupervised model to classify the institutions based on the I.D.E.A. variables I am able to identify. 
If I verify the existence of significant differences in enrollment predictions either across institution or across States depending on what ultimately is the frame of references, I would pursue these and try to identify modeling approaches that may explain and/or support the differences. 

## 8.	How do you plan to develop/apply ML and how you evaluate/compare the performance of the models?
The data will be extensive thus I am thinking that I may have to use a resource, such as Databricks, to be able to handle the data aggregately and efficiently. 
As far as the models’ performance is concerned, I would use the traditional indicators such as ROC curves, Silhouette Score etc. 

## 9.	What outcomes do you intend to achieve (better understanding of problems, tools to help solve problems, predictive analytics with practical applications, etc)?
I personally hope to develop my ability to manipulate a (large) dataset to come to interesting conclusions that may be then a small but useful contribution to the topic of education with respect to higher education in particular. 
It would be ideally very gratifying if I was able to find interesting information that could contribute to the discussion in the field of higher education, especially in connection to the challenges involving Inclusion, Diversity, Equity and Accessibility. 
