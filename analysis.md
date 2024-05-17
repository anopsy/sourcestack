# Job Search Optimization
## 1. Introduction
   Searching for a new job is one of those activities most people have to do, but only few are happy about it.
   Finding offers that look like your dream job is time consuming, and interviews can take up to several weeks in total.
   The ongoing AI revolution doesn't make it easier, especially for entry-level candidates like me. 
   
   ![image](https://github.com/anopsy/sourcestack/assets/74981211/77555441-f55e-4c3c-9da8-580462506f65)


## 2. Problem Statement
   Let's try to optimize the job search process. The problem is stated as follows.
   
   #### *How to maximize the benefits of a job and minimize the costs related to the search.*
   
   I'll define **the benefits in terms of financial and mental satisfaction** I'd have doing the job.
   We can measure the first one comparing compensation offered for a vacancy. Measuring the second one is a bit trickier,
   but it can be boiled down to well-being at work. It may encompass opportunities to learn and grow, good work-life balance,
   pleasant working atmosphere. A good approximation of the average satisfaction at a given company would be employee tenure.

   Thus, we can maximize our benefits by choosing to apply for jobs with compensation that fulfills our expectations and by checking what's the average job tenure at that company.

   How do we minimize **our costs - the time spent and mental load** related to searching for job offers and interviewing.
   In case of entry level jobs and the current situation on the job market (layoffs, rumours of LLM's replacing juniors), I was asking myself often a question:
   Are my skills enough to land a job? The answers depends mainly on how many jobs are available to Juniors and Interns.
   If the number of entry level job offers dropped down in the recent months, it would probably take me a longer time to get a job I wanted.
   If I'd spend that time working on making my stack more competetive or better alligned with employers, I could save myself months of stressful and futile interviews.

   We can minimize the cost of our job search by checking the trend of available entry-level jobs and if needed spend some of the time enhancing our skill set.

   Optimizing the job search consists therefore both of maximizing the financial and mental satisfaction reflected in the compensation and job tenure by choosing the jobs with maximal values, and
   minimizing the time spent and stress experienced while interviewing by adjusting your competetiveness if the job market situation requires it.
   
## 3. Dataset
   I'll try to answer the question I asked in the problem statement by analysing and modelling the data I obtained from SourceStack.
   I queried the API on June the 9th 2023 and April the 2nd 2024, getting 50_000 records on each day, resulting in a dataset with 100_000 records.
   The offers are mostly engineering jobs.
   
   ![image](https://github.com/anopsy/sourcestack/assets/74981211/992146c1-85ca-4ffe-bf65-e176a9fcf994)

   
   The dataset has 16 features:

   <br>job_name [str] - job title
   <br>job_location [str] - information about job location 
   <br>hours [str] - information about type of employment full-time/part-time/contract/gig
   <br>remote [bool] - information if the role is remote or not
   <br>company_name [str] - the name of the company
   <br>education [str] - what education is required
   <br>tags_matched/ tag/categories/categories list[str] - tags describing the job
   <br>seniority [str] - information about seniority
   <br>comp_est [str] - estimated compensation offered for this vacancy
   <br>language [str] - language required 
   <br>city [str] - city location of the offered job
   <br>country [str] - country location of the offered job
   <br>job_published_at [str] - the date at which the job was published
   <br>last_indexed [str] - the most current date the job was indexed at

   The dataset contains a significant amount of null values and only one duplicate.
   
   ![image](https://github.com/anopsy/sourcestack/assets/74981211/df8d965a-7d44-4edc-92a0-b342bae0029e)

   The job offers come from 183 countries with 44 languages and 7_795 different cities.

   Countries:

   ![image](https://github.com/anopsy/sourcestack/assets/74981211/3b8ced68-da33-4eb0-8f8d-012ffffa6d54)

   
   ![image](https://github.com/anopsy/sourcestack/assets/74981211/5095f61f-a8fc-478a-97b0-4662ffee480e)

   Top Countries being:

   <br>United States - 44_581 job offers
   <br>India - 10_275
   <br>United Kingdom - 4191
   <br>Germany - 3560
   <br>Canada - 2362
   

   Cities:
   
   ![image](https://github.com/anopsy/sourcestack/assets/74981211/3f5c10e6-8f9a-4ffb-af84-da78f2562827)

  Top Cities being:

  <br>Bengaluru with 1942 job offers in total.
  <br>Bangalore - 1512
  <br>San Francisco - 961
  <br>London - 956
  <br>Singapore - 863


   <br>The job offers come from 28_781 different companies.
   <br>The top 20 companies posted in total 9502 job offers - 9,5% of the total job offers.

   ![image](https://github.com/anopsy/sourcestack/assets/74981211/a7e32a3f-3fde-4466-94ad-b2476ca58068)
   
## 4. Optimization
### Minimizing the costs

  Has the situation on the job market changed and we will have to take measures to compensate for entry level jobs scarcity?
  Let's have a look at the comparison of number of entry level jobs in June 2023 and April 2024.

   ![image](https://github.com/anopsy/sourcestack/assets/74981211/6729d583-0a35-41ca-a9e1-c5e44c22b6cd)


  In June 2023 Junior job offers were 1.674% of the total 50000 
  <br>Internship offers were 1.504% of the total 50000

  In April 2024 Junior job offers were 2.118% of the total 50000 
  <br>Internship offers were 2.46% of the total 50000 

  Entry-level jobs (Junior + Intern) in June 2023 were 3.178% 
  <br>Entry-level jobs (Junior + Intern) in April 2024 were 4.578% 
  <br>but if we look closer, we can see a significant increase in the number of entry level jobs.
  <br>The number of entry-level jobs has risen by 44% !!!

  ![image](https://github.com/anopsy/sourcestack/assets/74981211/fc0f371a-461b-4f29-a2ee-0c28d83b49aa)

  Therefore we can see that compensating for scarcity on the job market will not be needed, as there are more jobs available now.






### Maximizing the benefits
### WIP
## 5. Conclusions
### WIP
