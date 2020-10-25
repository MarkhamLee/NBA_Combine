# Is the NBA Combine an Effective Predictor of In Game Performance?

By: Markham Lee

This was a project for my CSE163 - Intermediate Data Programming Course at the University of Washington. The goal of the project was to study the data coming out of the NBA Combine event (where the raw athletic ability of NBA draft prospects are measured through a series of events meant to test their agility, speed, strength and jumping ability), to see if there was any relationship between those measures of athleticism and on court performance. The project was inspired by NBA superstar [Kevin Durant](https://abcnews.go.com/Sports/kevin-durant-calls-nba-combine-waste-time-top/story?id=47338234), who had a historically bad performance at the combine but is already a future hall of fame who has won multiple championships. He claims that the combine is "meaningless", and this analysis is a an attempt at seeing if he's right via analyzing the data for the past ten NBA seasons. Another component of the project was to evaluate the general effectiveness of the NBA's methods for evaluating prospects, by looking at draft position vs. in game performance after reaching the NBA. *I.e. are draft busts rare are they closer to the norm?*

The version posted has some rather significant updates vs. the one I did for my class, including updated analysis related to the number of players above the average for points per game and win shares and those in the 75th percentile for same and how that relates to the combine scores and draft position. The report PDF is also significantly streamlined as the original report contained items that were very specific to the assignment rubric, and aren't particularly relevant outside of the class. Items called out in *"update information"* are items I specifically added to the project after I turned it in, in order to enhance it as a portfolio project.

This project makes heavy use of Jupyter Notebooks, however, if you don't have the environment for Jupyter Notebook, [Binder](https://mybinder.org/) is a free open source tool that can read a directory containing Jupyter Notebooks and provide a browser based environment to run them in.

**Included in this repository are the following files:**

* NBA_Project(Revised).ipynb is the Jupyter notebook that contains the original code and some additions I made after I had turned the project in. It also has additional analyses/write-up embedded into it. This is the primary source of the code for this project, and is more up to date than the individual python files.
* NBA_Project(Revised).pdf is a PDF version of the Jupyter Notebook, easier to consume for people that want to see the code but may not have a Jupyter environment.
* NBA_Report(FINAL).pdf is a detailed report of the project's findings: inclusive of visualizations, analysis, caveats and discussion of potential future enhancements. Those looking for results and analysis should look at this file.
* high_level_summary(FINAL).pdf is a more academic style summary, it goes into more depth on the reasoning behind doing the project, research questions, methodology and problems encountered and provides a high level summary of the results. It's the "why and the how" more than it is a deep dive into the results.
* nba_stats contains the files with NBA player statistics
* new_data contains the file with the NBA Combine information
* data_analysis.py contains the code that generates all of the visualizations, it's the original code from the assignment, save the additional code I added to the Jupyter notebook
* data_processing.py contains the code for ingesting and cleaning the data
* If you want to run the analysis with the python code directly just run everything from the visualization file, as it will call the ingestion file when necessary. In Visual Studio code I would just right click and select "run the file"  
* Visualizations - contains the visualizations created by the original version of the project

**Python Packages Information:**

* Pandas for data frame interactions
* OS for accessing a file directory
* glob2 for opening multiple CSV files and quickly aggregating them into one data frame
* matplotlib and seaborn for the visualizations
* numpy and sklearn are listed in the jupyter notebook but not used since regression and/or ML ended up not being necessary. I left them there as I may use them in future versions

**Development Tools & Language Information:**

* Managed the python environment and packages with Anaconda
* IDE: Visual Studio Code for Python and Markdown file editing
* Jupyter Notebook
* Flake8 for code hygiene and lintiing the .py and .md files created in Visual Studio Code

## Update Information

#### 10-25-2020

* Added PDF version of Jupyter Notebook
* Put this into its own repo instead of it being a directory under the portfolio repo

#### 9-08-2020 NBA_Project(Revised)

* Added overview of the results (PPT saved as a PDF - NBA_report(FINAL).PDF)
* Updated Jupyter Notebook, small tweaks + additional visualizations

#### 9-02-2020 NBA_Project(Revised)

* Word smithing
* Refreshed source data just to be doubly sure, no changes to findings
* Updated findings to note wingspan vs. blocks as that was a near (0.67) strong relationship
* Added high level PDF summary of findings

#### 9-1-2020 NBA_Project(Revised)

* Added analysis related to number and % of athletes selected with the first 15 picks of the draft that performed above the league average in win shares and points per game
* Added significance tests for PPG, I.e. is there any difference in the proportion of players above and below the average
* Added analysis around the number of players selected with the first 15 picks of the draft that performed in the 75th percentile

#### Future changes

* ~~Add a PDF file that's a high level summary of all findings replete with visualizations~~ COMPLETE
* ~~Add a static version of the Jupyter Notebook~~ COMPLETE
* Use the NBA API to gather a larger data set, extended the in game player statistics out to 20-30 seasons
* Add combine data for a similar time frame as above
* Repeat this analysis for the WNBA (if possible) and see if the patterns observed in the NBA data are similar to what's observed in the Women's game.
