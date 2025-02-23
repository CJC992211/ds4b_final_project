# Final project for Data Science for Biologists, Fall 2021

This is a README file, written in _markdown_. README files are commonly part of disseminated software/code packages. They help to explain the contents of the software package: what files are what? how do you use the software? etc.

**[Instructions for final project](https://sjspielman.github.io/datascience_for_biologists/homeworks/project/project_proposal_instructions.html)**

Final Project Proposal and Final Project Instructions
Data Science for Biologists, Fall 2021
Overall Instructions
Project Proposal Instructions
Final Project Instructions



Overall Instructions
For your final project, you will be analyzing a dataset of your choosing. Your goal will be to ask FOUR scientific/explanatory questions about your dataset, and answer each question with any necessary associated wrangling, modeling, and visualization to address and/or complement the question.

Ground rules
You must complete your project each using the respective Rmarkdown template, and it must knit without errors for full credit. The template should knit to HTML only.
Your Rmarkdown document must use an Rmarkdown document theme and code syntax highlighting theme of your choosing.
Every question requires a data visualization. It does not matter which geoms you use for your plots, as long as the plots are properly made and are relevant to address or complement your given exploratory question.
In other words: IT IS OK if you have the same type of plot for multiple questions, as long each plot is appropriately relevant for your question!
Carefully go over any HW feedback you have received for exploratory analysis to prepare!!
You must ensure that all rendered plots are fully visible and legible with an appropriate aspect ratio.
At least ONE question must be EITHER a linear model or logistic regression. You can do more models if you want, but only one is required on the project. Associated ground rules:
You do not need to use testing/training splits for model training and validation, but you can if you choose. If you do this, you must ensure your random number seed is properly set, and your written text and code output are precisely consistent.
You can either do a specific hypothesis-based analysis (your question is: “do these specific variables explain variation in/predict status of response?”, for linear/logistic respectively) OR use model selection to determine predictors (your question is: “does the model explain variation in/predict status of response?”).
If you perform model selection, make it easier on yourself: Use step() to perform model selection, and consider the literal output of using step() to be your model itself. End of story!
For any linear models, your explanation must include a brief interpretation of the model’s RMSE and R2. You are not required to interpret coefficients. There are several options for how you can include a visualization for this question, which we will discuss together based on your circumstance if you decide to include a linear model. Because you are not likely to be doing training/testing, it is only possible to evaluate model performance (% explained and error). Overfitting is only possible to learn about with validation procedures, so this is not part of your project (unless you decide you want to do a validation procedure!)
For any logistic regressions, your explanation must include a brief interpretation of the model’s AUC. Your visualization must be the logistic curve itself.



Project Proposal Instructions
Due Wednesday 12/1/21 by 11:59 PM. Timely submission is extremely important in case there are problems with your data’s suitability for the final project and you need to find a new one. As long as you submit a complete proposal by the deadline, you will be able to resubmit the proposal for a full regrade if I do not approve it.

For your proposal, you will identify a dataset to analyze, using the provided template. You must choose a dataset that we have NOT used in class and you have not personally used for a #tidytuesday extra credit Some fantastic options for finding data include:

The #tidytuesday repository has a dataset for each week since 2018.
https://github.com/rfordatascience/tidytuesday
The statistics website FiveThirtyEight has a bunch of datasets they have compiled (some of which have been used as #tidytuesday, actually!)
https://data.fivethirtyeight.com/
The website “Kaggle” has a lot of compiled datasets. Depending on the dataset, you may need to make a free account on the website to download the data, but you do NOT have to pay.
https://www.kaggle.com/datasets
The Gapminder website has a lot of great datasets
https://www.gapminder.org/data/
The UCI Machine Learning database
https://archive.ics.uci.edu/ml/datasets.php
This website lists a bunch of other options
https://www.dataquest.io/blog/free-datasets-for-projects/
If you have read a scientific paper that you think has accessible data you want to use, please reach out to me and I will help you track it down!
If there is a specific of data from a certain field you want to use but you don’t know where to find it, reach out to me and I will help see if I can find one for you!
If you find multiple related datasets from the same source (e.g. some #tidytuesday datasets have several CSVs associated with them), you can use them all and consider it “one” dataset.
For your proposal, you will…
Use the template!!
Introduce and briefly describe your dataset:
Provide a brief description (in your own words! do not plagiarize!!) of the data itself so anyone who views your analysis has a solid grounding to understand what you are doing!
Explain what excites or interests you about this data! Why did you choose it?
Include an properly-formatted markdown link to the source of the data. Properly formatted markdown links are formatted as: [text you want displayed](link). Please refer to the file activities/rmarkdown_demonstration.Rmd for further help.
Read in the dataset with read_csv() and display the dataset with the dplyr::glimpse() function.
Your dataset will either be a literal file, or it may be available online as a URL (like the #tidytuesday datasets). If it’s a URL, just read from URL as normal.
If your dataset is a literal file and CANNOT be read from a URL directly, you MUST take the following actions:
Ensure the name of your file (and hence the code to read it in) is called yourlastname_dataset.csv (or a different extension as appropriate). For example, I would name my data file as spielman_dataset.csv.
Submit the dataset to Canvas along with your Rmd (multi-file submission.) If the data is not also provided, the Rmd will not knit, and you will not be able to get credit.
Include either a bullet point list or a table (learn how to make a markdown table using resources embedded in activities/rmarkdown_demonstration.Rmd) that briefly describes all the variables (columns) in your data. If you obtained your data from a website that already contains such a bullet list or table description, feel free to literally use the same wording.
If there’s an insane amount of columns in your data such that this is ridiculous (like 30+ columns), please talk to me about it.
Indicate which variable you plan to model and whether you will be using linear or logistic regression. (Hint: it entirely depends on the type of data!)
FOR BONUS POINTS!! (CONCERNED ABOUT YOUR GRADE??!?! DOING THIS BONUS WILL SERIOUSLY HELP! THIS!!)
Also tell me (casually is ok!) the other three questions you are considering asking for your final project, and to the extent possible, tell me about what kind of plot you are thinking of making.
Doing this bonus means I will give you direct feedback on your project ideas while I grade the proposal! We can even use this bonus to start a back-and-forth conversation (after this submission, can continue on Slack!) about how you can approach each of your questions. This initiative will set you up for much more success completing the project!
If you want to up your game more, you can literally do your whole project effectively for a completion grade, and my grading feedback will guide you to what steps you need to take to tweak work you’ve started to really crush the final project.
Punchline: Get bonus credit to put in more effort for the proposal so that you can put in less effort on the final project AND likely get a better grade on the final project.



Final Project Instructions
Complete and push all code by Tuesday 12/14/21 by 11:59 PM. Whatever code you most recently pushed before this time will be your final submission. To be clear: Even if you push commits AFTER the deadline, those code changes will not be considered at all.

Unless you have an extremely extuenuating circumstance that we specifically discuss (in which case you are likely to get an “Incomplete” grade for the class), there are NO EXTENSIONS WHATSOEVER because this is equivalent to a “final exam.”

You must complete your final project using the template Rmarkdown file in your copy of the final project Github repository, which we will setup together as a class activity.
Repository instructions
Your final repository should contain only these files:

README.md (I have written this file for you)
The .gitignore file (I have written this file for you)
The final_project.Rproj file associated with the project
DO NOT WORRY if this file has unstaged changes throughout your work. NOT A BIG DEAL if you end up adding/committing or not!
Your final project as an Rmarkdown named <lastname>_final_project.Rmd.
For example, I would call this spielman_final_project.Rmd. If you have two last names, you may use a dash: last-name_final_project.Rmd or choose to use only one - whichever you prefer!
Your final knitted project <lastname>_final_project.html (should be automatically named correctly if the Rmd is named correctly!)
Your dataset named <lastname>_dataset.csv (or .tsv, etc. depending on the file type)
Unless your data is being directly read in from a URL. If it’s accessible from a URL, there does not need to be a separate file included in your project.
A directory called figures/ which contains all figures you have made in PNG format. Figures must be named as: questionX.png, and if there are multiple figures per question, questionX_figureY.png (where X and Y are numbers).


Template
The project is templated out for you as follows:

The Introduction section should first briefly describe the dataset (you can use the exact text you used in the proposal), including a direct link to the data’s source. You should then include code to read in and briefly explore the dataset so readers have a sense of the data. Again, if you are reading data from a file, make sure the file is properly named.

For each Question section, you should provide your question (questions are questions, not tasks) as a level-4 header. Under the Methods sub-header, include named code chunk(s) you need to wrangle and visualize data to answer the question and make your plot(s). Chunks should be reasonably named for the given task, and you can have as many chunks as you want as long as they are all under Methods and you ensure that plot(s) are revealed as the last piece of code output in Methods. Then, under the Answer sub-header, provide your brief answer to your question.

Remember! At the top of these instructions are associated ground rules for doing your modeling!

All figures must be both shown in the Rmd AND saved to a separate file inside a directory called figures/. Figures must always be fully visible and legible which will require you to set proper figure sizes

Export: Figures must be exported as PNG files to the figures/ directory and named as questionX.png where X is the question number. If there are multiple figures for the question, use questionX_figureY.png (like question1_figure1.png and question1_figure2.png for example).
ggsave() must be used as taught here
You must use the variable path_to_figures (defined in setup chunk) along with the function file.path() when using ggsave() to export figures.


How will you be graded?
This project is worth 20% of your final grade and is worth 150 points as follows:

20 points for each (total is 4x20=80) successfully-completed question and answer, where each question/answer must have at least one associated figure that is both revealed and exported.
20 points for adhering to the format. This includes…
Placing code into their intended code chunk. For example, libraries should only be loaded in the setup code chunk.
Naming all code chunks
Proper use of the file.path() function with the path_to_figures variable when exporting figures
NOT using “forbidden” code like View(), install.packages(), etc. If you need to use other packages that aren’t already installed, please talk to me first!
Setting your favorite Rmarkdown theme and syntax highlighting theme. Note that the template does not contain a default, so you must set your themes.
Ensuring all markdown elements appear in the knitted output as intended.
50 points for successfully completing the project with git version control
6 points are for your six required commits (total 36 points)
14 points for a properly organized repository with correctly named files according to instructions
If you do not use git for your final project (i.e. you write an Rmarkdown and email it to me by the deadline), you can still get credit for your final project, BUT your maximum possible grade will be 100/150 (66.7%) since those 50 points are automatically lost.
