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
	- 
* How is the school summary affected?
* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
* How does replacing the ninth-grade scores affect the following:
* Math and reading scores by grade
* Scores by school spending
* Scores by school size
* Scores by school type

![Code Section 1](https://github.com/coxjack/PythonChallenge3/blob/main/Additional%20Supporting%20Images/code_pt_1.png)
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
