# FunData-Assessment

Fundamentals of Data Analysis:

In this readme, I have both readmes for the module included, these are also individually in the folders for both parts of the module. 



Weekly Tasks:
There is 5 topics covered in this module:

1. Information
2. Randomness
3. Bias
4. Outliers
5. Cleansing

All my workbooks have redo_ prefixing them, as I had some issues with jupyter notebooks not saving my updates and losing some information. 
I had to download my workbooks when they were complete and readd them to the path to avoid loss of work. 

Topic 1: Information

Exercise 1:

Adjust existing code to now generate 1000 charater long string with weights based on 2 Characters

For this exercise I took the existing code, and modified it to accept 2 previous characters:
threghts = {c+d: {e: sbook.count(c + d + e)  for e in chars} for d in chars for c in chars}

This allowed me to print out character based on 2 previous letters, The flaw with this is the chapters use roman numerals. iii is one of the only instances of 3 i’s in a row. 
If i characters start printing the program can get stuck only printing i’s. 


Exercise 2: 
Find out why the log of 0 is undefined? 
Explained in the notebook using LaTex.

Topic 2 Randomness: 
Randomness Exercise 1
It is somewhat interesting that (5 * 4 * 3 * 2 * 1) perfectly divides (10 * 9 * 8 * 7 * 6) - there's no remainder.
If we only wanted exactly four heads as opposed to five, the equivalent calculation would be (10 * 9 * 8 * 7) / (4 * 3 * 2 * 1).
Does that evenly divide too? What is the formula in general?
Does it always come out as a positive whole number?

Exercise 2: 
Note that there are the same number of ways to get 4 tails as there to get 4 heads. Explain why this is.
Exercise 3
Plot bar charts or histograms of any three different distributions listed at the following link:
https://numpy.org/doc/stable/reference/random/generator.html#distributions

All topic 2 exercises are completed in the notebook, Exercise 3 the plots are done from the link above. 

Topic 3: Bias

Bias Exercise 1
Give three real-world examples of different types of cognitive bias.
I explain 1. Dunning-Kruger Effect, 2. The Hindsight Bias, 3. Anchoring Bias.
Initially I had other examples picked, but this exercise is the first time I had saving issues in Jupyter, I had to redo this work. 

Bias Exercise 2
Show that the difference between the standard deviation calculations is greatest for small sample sizes. I explained this difference using the example code give to us where 2 sets of numbers had the same mean, but one outlier caused one group to have a much larger standard deviation. 


Topic 4: Outliers
Exercise 1:
Create box plots on a single set of axes for all five experiments in the morley data set.

I referred back to my own project using the iris data set from last semester to reuse some pandas code for this topic
https://github.com/RochejamieGMIT/pands-project
I used pandas for this topic as it is easier to deal with pandas data frames to create plots. 

Exercise 2:
Create box plots for all of the numercial variables in Fisher's Iris Data Set.
I used pandas to create these plots, I also gave the data set columns headings for ease of creating the plots. 

Exercise 3:
Adapt the above code and plots so that the overall plot is inversely propertional and the individual groups are directly proportional.
For the below code, I took the code that was given in the notebook, and inverted the Y value when adding the noise.
I was going to try plot $-x$ against $y^2$, to get the inverse proportional curve, but  the best fit did not work, the best fit line would not fit the plot. I could not get the polynomial line to fit the curve. 

Topic 5: Cleansing
Exercise 1
Write a Python function to remove all non-alphanumeric characters from a string.
Create raw string for regular expression, any charatcer that is not/complement of (^) a-zA-Z0-9, 
Not using the \W version expression as it includes _ 

Exercise 2:
Adapt the above code to capitalise the first letter of the iris species, using regular expressions.
For this exercise I could not adapt the code to change the letter to capital using the reg ex properly. 
I tried a few different things, but eventually added a .capitalize() string method to the line that was given in the notebook. 
I think there maybe a more correct way to implement this with out the .capitalize() method, but I could not get it to work. 



Normal Distribution Project:

For the normal distribution project I started with an intial history of the development of the normal distribution.

After the history introduction I I cover the technical explanation and the formula. 

Supported with graphs and code to display the normal distribution. 

After dipicting the normal distribution, I go through using stats.normaltest(s) and kurtosistest(s) to test the generated data for normal distribution. 

And finally list and very briefly explain some further test methods available. 


References For Weekly tasks:
https://www.gutenberg.org/files/11/11-0.txt

https://tex.stackexchange.com/questions/238179/epsilon-and-log-functions

https://latex.org/forum/viewtopic.php?t=15419

https://en.wikipedia.org/wiki/Equals_sign#:~:text=almost%20the%20same.%22-,Not%20equal,the%20%22%5Cneq%22%20command.

https://math.meta.stackexchange.com/questions/22385/latex-symbols-for-therefore-and-suchthat#:~:text=You%20should%20use%20the%20ASCII,%22%20and%20%22such%20that%22.&text=%E2%88%B4%20means%20%22therefore%22%2C%20and,implies%22%20and%20is%20a%20verb.

https://numpy.org/doc/stable/reference/random/generator.html#distributions

https://numpy.org/doc/stable/reference/random/generated/numpy.random.Generator.geometric.html#numpy.random.Generator.geometric

https://numpy.org/doc/stable/reference/random/generated/numpy.random.Generator.noncentral_chisquare.html

https://numpy.org/doc/stable/reference/random/generated/numpy.random.Generator.logseries.html

https://www.towergateinsurance.co.uk/liability-insurance/cognitive-biases

https://www.verywellmind.com/cognitive-biases-distort-thinking-2794763

https://www.titlemax.com/discovery-center/lifestyle/50-cognitive-biases-to-be-aware-of-so-you-can-be-the-very-best-version-of-you/

https://www.simplypsychology.org/cognitive-bias.html

https://github.com/RochejamieGMIT/pands-project

https://vincentarelbundock.github.io/Rdatasets/csv/datasets/morley.csv

https://stackoverflow.com/questions/39399712/delete-pandas-column-with-no-name

https://www.geeksforgeeks.org/box-plot-visualization-with-pandas-and-seaborn/

http://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data

https://www.geeksforgeeks.org/how-to-add-header-row-to-a-pandas-dataframe/

https://www.geeksforgeeks.org/capitalize-first-letter-of-a-column-in-pandas-dataframe/?ref=rp

https://favtutor.com/blogs/capitalize-first-letter-python

https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data




References for Normal Distribution:

https://www.khanacademy.org/math/statistics-probability/modeling-distributions-of-data/normal-distributions-library/a/normal-distributions-review

https://www.khanacademy.org/math/ap-statistics/density-curves-normal-distribution-ap/density-curves/v/median-mean-and-skew-from-density-curves

https://www.khanacademy.org/math/ap-statistics/density-curves-normal-distribution-ap/stats-normal-distributions/v/ck12-org-normal-distribution-problems-qualitative-sense-of-normal-distributions

https://statisticsbyjim.com/basics/normal-distribution/

https://corporatefinanceinstitute.com/resources/data-science/normal-distribution/

https://www.itl.nist.gov/div898/handbook/eda/section3/eda35b.htm

https://www.mathsisfun.com/data/standard-normal-distribution.html

https://en.wikipedia.org/wiki/Normal_distribution#Definitions

https://www.google.com/search?q=normal+distribution+definition&rlz=1C1ONGR_enIE933IE933&oq=normal+distribution+def&aqs=chrome.0.0i512j69i57j0i512l5j69i60.15472j0j7&sourceid=chrome&ie=UTF-8

https://www.techtarget.com/whatis/definition/normal-distribution

https://www.statology.org/plot-normal-distribution-python/

https://en.wikipedia.org/wiki/Mean#Statistical_location

https://en.wikipedia.org/wiki/Standard_deviation

https://www.z-table.com/history-on-normal-distirbution.html#:~:text=The%20origin%20of%20normal%20distribution,probability%20distribution%20of%20coin%20flips.

https://sphweb.bumc.bu.edu/otlt/mph-modules/bs/bs704_probability/BS704_Probability12.html#:~:text=The%20central%20limit%20theorem%20states,will%20be%20approximately%20normally%20distributed.

https://onlinestatbook.com/2/normal_distribution/history_normal.html

https://towardsdatascience.com/6-ways-to-test-for-a-normal-distribution-which-one-to-use-9dcf47d8fa93#:~:text=For%20quick%20and%20visual%20identification,use%20the%20Shapiro%20Wilk%20test.

https://encyclopediaofmath.org/wiki/Kolmogorov-Smirnov_test

https://variation.com/wp-content/distribution_analyzer_help/hs141.htm

https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.normaltest.html

https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.kurtosistest.html

https://www.statology.org/z-value-vs-p-value/

https://docs.scipy.org/doc/scipy-1.2.0/reference/generated/scipy.stats.kurtosistest.html

https://variation.com/wp-content/distribution_analyzer_help/hs133.htm#:~:text=The%20normal%20distribution%20has%20a,than%20or%20equal%20to%200.05.

https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.normaltest.html

https://osf.io/tz48r/download#:~:text=Thus%2C%20if%20you%20reject%20the,your%20data%20is%20normally%20distributed.