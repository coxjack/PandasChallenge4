## School District Analysis
Challenge 4 for Butler Data Science

## 1. Overview of School District Analysis
### 
* The goal of this module is to assist a city school district with their analysis of student funding and student standardized test scores. In our analysis summarized the following:
	1. The top 5 and bottom 5 performing schools, based on the overall passing rate
	2. The average math score for each grade level from each school
	3. The average reading score for each grade level from each school
	4. The scores by school spending per student, by school size, and by school type
	5. Summaries of the district as a whole and the per school averages

## 2. Results
### 
* How is the district summary affected?
	- We removed 461 student grades and recalculated the passing scores. The passing scores did go down very slightly. Math from 75 to 74.8. Reading from 86 to 85.7 and overall passing from 65 to 64.9 

	  - Original District summary

![Original district summary df](https://github.com/coxjack/PandasChallenge4/blob/main/additional%20supporting%20images/Original%20District%20Summary.png)
	
	  - Refactored District summary

![Refactored district summary df](https://github.com/coxjack/PandasChallenge4/blob/main/additional%20supporting%20images/Refactored%20District%20Summary.png)


* How is the school summary affected?
	- The only school affected in the per school summary is obviously Thomas High because it is the only school that had adjustments to student's grades. There were small changes in their passing scores. Passing math scores went down .1 percentage points, passing reading scores went down .3 percentage points and overall passing scores went down .3 percentage points.

	  - Original Per School summary

![Original Per School summary](https://github.com/coxjack/PandasChallenge4/blob/main/additional%20supporting%20images/originalperschoolsummary.png)
	
	  - Refactored Per School summary

![Refactored Per School summary](https://github.com/coxjack/PandasChallenge4/blob/main/additional%20supporting%20images/refactored%20per%20school%20summary.png)

* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
	- Although there are small changes to the passing scores at Thomas High school, this does not change the school's performance relative to the other schools in the district. It was the number two school before the removal of ninth grade scores and remains the number two school after the removal.

	  - Original Top 5 Schools

![Original Top 5 Schools](https://github.com/coxjack/PandasChallenge4/blob/main/additional%20supporting%20images/original%20top%205.png)
	
	  - Refactored Top 5 Schools

![Refactored Top 5 Schools](https://github.com/coxjack/PandasChallenge4/blob/main/additional%20supporting%20images/refactored%20top%205.png)

* Math and reading scores by grade
	- The only change to the scores by grade is the Thomas High School ninth graders now display a NaN instead of their original scores. This applies to both math and reading since both scores were removed.
	  - Original math scores by grade

![Original math scores by grade](https://github.com/coxjack/PandasChallenge4/blob/main/additional%20supporting%20images/original%20math%20scores%20by%20grade.png)
	
	  - Original reading scores by grade

![Original reading scores by grade](https://github.com/coxjack/PandasChallenge4/blob/main/additional%20supporting%20images/orginal%20reading%20scores%20by%20grade.png)

	  - Refactored math scores by grade

![Refactored math scores by grade](https://github.com/coxjack/PandasChallenge4/blob/main/additional%20supporting%20images/refactored%20math%20by%20grade.png)
	
	  - Refactored reading scores by grade

![Refactored reading scores by grade](https://github.com/coxjack/PandasChallenge4/blob/main/additional%20supporting%20images/refactored%20reading%20by%20grade.png)

* Scores by school spending
* Scores by school size
* Scores by school type


![Code Section 2](https://github.com/coxjack/PythonChallenge3/blob/main/Additional%20Supporting%20Images/code_pt_2.png)
![Code Section 3](https://github.com/coxjack/PythonChallenge3/blob/main/Additional%20Supporting%20Images/code_pt_3.png)

## 3. Election Audit Summary
### 
* Applying this script to any election audit is easy. The first thing we would need to do is import from whatever results file we would have. 
	- Add a variable to load a file from a path.
	  - ***Original Script***
	    - file_to_load = os.path.join("Resources", "election_results.csv")
	  - ***Modified Script***
	    - file_to_load = os.path.join("Any_election_results.csv)
* If this was a national election we could instead gather votes by state.
	- Create a list and votes dictionary
	  - ***Original Script***
	    - county_options = []
	    - county_votes = {}
	  - ***Modified Script***
	    - state_options = []
	    - state_votes = {}
