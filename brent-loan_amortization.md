## Step 1: Brainstorming 

This part of the 'Course Spec' process is designed to help guide you through course design by having you think through several key questions. Please make sure to delete the examples provided here for you.

### A. What problem(s) will students learn how to solve? (minimum of 5 problems)

- [ ] Write a list of ideas for problems that the students will encounter in the course.
> From a course on spreadsheets for finance:
>
>- How to design a Google Sheets interface to analyze the past performance of a stock 
>- How to display the past evolution of a stock price
>- How to compute stock returns
>- How to measure historical performance and risk
>- How to display the distribution of historical returns
>- How to model stock returns using the Gaussian assumption
>- How to use a benchmark to assess the risk and return of a stock


### B. What are the learning objectives of the course?

- [ ] Write a list of learning objectives for the course. These are not shown to the students, but they will be used to ensure your vision for the course aligns with the vision of your Curriculum Lead.

>Example from our scikit-learn course:
>
>- Learn the key concepts of supervised learning and how to implement them on real-world datasets;
>- Learn to distinguish regression from classification problems;
>- Learn to evaluate how well your classification and regression modes perform;
>- Learn best practices in supervised learning, such as splitting into test/train sets and k-fold cross validation;
>- Learn how to improve model performance by both preprocessing your data and regularizing your models.


### C. What functions will students use? Please be exhaustive.

- [ ] Write a list of ideas for the Spreadsheets functions that you want to use in the course. Please note that we packages, currently cannot support Google Sheets add-ons. If there are any important functions, methods, or commands that you want to teach, you can mention them here.

> Example from a course on spreadsheets for finance.

> Basic Google Sheets functions: SUM, PRODUCT, COUNT, IF, COUNTIF, AVERAGE, MIN, MAX, STDEV, PERCENTILES, ARRAYFORMULA,
> VLOOKUP, NORMDIST, NORMINV, CORREL.


### D. What terms or jargon will you define?

- [ ] Write a list of technical terms, jargon, and acronyms that will be used in the course and define them as well.

> Example from a course on pandas.
>
> - Tabular data: data with rows and columns
> - DataFrame: a pandas representation of tabular data
> - Merge: an opperation that combines two DataFrames based on common column values
> - Aggregate: a single value computed based on a set of values.  For example, an average applied to a column of numbers is an aggregate function

### E. What analogies or heuristics will you use?

- [ ] Write a list of analogies for concepts, heuristics for best practices, and any other non-technical explanations of things that may be helpful to students _(minimum of two)_.

>Example from a course on forecasting product demand. This analogy is likely intuitive to most people.
>
>Signal and noise - It's like trying to hear someone across a crowded room. Remove the noise, and you can easily understand what they are telling you.


### F. What mistakes or misconceptions do you expect? 

- [ ] Write a list of common mistakes _(minimum of two)_ that you think students will make. These can be programming mistakes, conceptual misunderstandings, or simply examples of things that are unintuitive. 

>Example from a course on generalized additive models:
>
>The difference between prediction intervals and confidence intervals.


### G. What datasets will you use? 

- [ ] Write a list of datasets that you will use in the course, a short description of each dataset (if it's not clear from the title), how you intend to use it and include a link to its source(s). You should aim to have between 1 and 8 datasets in your course.

Please avoid [overused datasets](https://authoring.datacamp.com/courses/design/brainstorming-datasets.html).

## Step 2: Who is this course for?

Terms like "beginner" and "expert" mean different things to different people, so we use personas to help instructors clarify a course's audience. When designing a specific course, instructors should explain how it will or won't help these people, and what extra skills or prerequisite knowledge they are assuming their students have above and beyond what's included in the persona.

- [ ] Please select the learner personas that align with your course. 
- [ ] Include an explanation describing your reasoning behind choosing the corresponding learner persona and any other relevant information.

Choose the appropriate learners for your course by following this link to [learner personas](https://instructor-support.datacamp.com/courses/course-design/learner-personas)

* Learner persona 1: explanation
* Learner persona 2: explanation
* Learner persona 3: explanation

## Step 3: Course outline

A typical course is structured as follows:

- Chapter 1 has three lessons. This chapter is shorter than the rest since it serves as an introduction to the topic.
- Chapter 2 has 3-4 lessons.
- Chapter 3 has 3-4 lessons.
- Chapter 4 has 3-4 lessons.

A typical lesson is comprised of:

- A video exercise with slides and script, e.g. [sample video exercise](https://spreadsheets.datacamp.com/courses/intermediate-spreadsheets-for-data-science/chapters/working-with-numbers/exercises/5).
- 2-4 exercises that review what is covered in the video exercise.

*Remind yourself about [course terminology](https://authoring.datacamp.com/courses/design#terminology-and-structure), then describe the flow of the course.*

> Example from a course on spreadsheets for finance

> Chapter 1 - Monitoring historical prices
> In this first chapter, you’ll be introduced to the problem: you have a time series of monthly (historical) prices for the stock ABC from which you have to extract some meaningful information. You’ll be given some definitions (what is a stock? what are dividends?), and at the end of the chapter, you’ll be able to graphically represent the evolution of a stock price over a specific period.

>   * Lesson 1.1 - Historical prices and first metrics
>     * A learning objective: Identify relevant information of stock prices and dividends for a specific time period.
>     * Description: You’ll be introduced to the dataset. You’ll learn what is a stock, why its price changes over time, what are dividends and when a company decides to pay them out. Once the theoretical part is done, we’ll provide you with the first set of indicators to look at when dealing with a time series of historical prices for a stock: minimum, maximum and average price. At the end of the chapter, you’ll learn how to compute them using the functions MIN, MAX, and AVERAGE.
>     * Some functions introduced/used: COUNT, MIN, MAX, AVERAGE, COUNTIF, MINIF, MAXIF, AVERAGEIF
>   * Lesson 1.2 - Identifying dates with unusual prices
>     * A learning objective: Identify dates when extreme prices occurred using the LOOKUP function.
>     * Description: Once having obtained the extremes of the ABC price during the period under analysis, in order to have more and better insights, it is crucial to know when these extremes occur, at which dates. Then, you’ll learn how to use the VLOOKUP function.
>     * Some functions introduced/used: VLOOKUP
>   * Lesson 1.3 - Visualizing the price evolution
>     * A learning objective: Display the evolution of the price using standard plotting functions and include in the graph additional indicators such as minimum, maximum and average price.
>     * Description: We build the first interface. It’s time to put all together and show it in a meaningful chart. 
>     * Some functions introduced/used: Google Sheets plots

> Chapter 2 - Monitoring historical returns
> In this chapter, the core of the analysis will switch from historical prices to historical returns. You’ll learn (and compute) the main performance indicators of past returns, both in terms of reward and risk. Finally, you’ll be introduced to risk-adjusted performance measures: indicators that take into account both reward and risk.

>   * Lesson 2.1 - From prices to returns
>     * A learning objective: Understand what is a financial return and compute returns from a time series of historical prices.
>     * Description: You’ll go through the concept of financial returns. What is a return? How is it computed?
>     * Some functions introduced/used: Simple division operator /, drag formulas, format with %
>   * Lesson 2.2 - Performance metrics
>     * A learning objective: Identify and compute both geometric, and arithmetic mean return using the functions AVERAGE, PRODUCT, ARRAYFORMULA, and GEOMEAN.
>     * Description: You’ll learn how to compute the effective rate of return of an investment, that is, the geometric mean return. Depending on the purpose of your analysis, you might also want to compute the arithmetic return, which is a simple indicator of the expected return you can get from that investment. Finally, there will be a brief explanation of the spreadsheet function that can be used to compute these metrics.
>     * Some functions introduced/used: AVERAGE, PRODUCT, ARRAYFORMULA, GEOMEAN
>   * Lesson 2.3 - Risk metrics
>     * A learning objective: Identify and compute key risk measures using functions such as STDEV and PERCENTILE.
>     * Description: You'll be introduced to the risk side of owning a stock. First, we’ll talk about the standard deviation, aka the volatility of the stock price over time. Maybe the most used risk indicator. Then, we’ll start having a look at the returns as a series of sorted values, and we’ll introduce the concept of percentiles, which can be used to define other popular risk-indicators (IQ ranges, historical VaR).
>     * Some functions introduced/used: STDEV (unbiased), PERCENTILE
>   * Lesson 2.4 - Risk-adjusted metrics
>     * A learning objective: Compute performance metrics that take risk into account.
>     * Description: In the final lesson of this chapter, you’ll be introduced to risk-adjusted indicators. Such indicators reveal how much risk was taken to achieve a return. In particular, we’ll focus on one of the most common risk-adjusted metric, the Sharpe Ratio.
>     * Some functions introduced/used: STDEV (unbiased), PERCENTILE

> Chapter 3 - Monitoring the distribution of returns
> In this chapter, you'll look at the full distribution of historical returns. First, you’ll learn how to build a histogram to describe the distribution of historical returns. Second, you’ll be introduced to the Gaussian distribution, a commonly used model for stock returns. You'll visually inspect if the Gaussian model is reasonable for the ABC stock returns. Finally, you'll understand potential flaws with the Gaussian model.

>   * Lesson 3.1 - Histogram of stock returns
>     * A learning objective: Create a histogram for the stock returns.
>     * Description: The learner will be driven step by step in the process of creating a histogram describing the distribution of past stock returns. After the graph has been generated, we’ll give the definitions of two indicators that describe the shape of a statistical distribution, that is, skewness and kurtosis.
>     * Some functions introduced/used: COUNTIF, (FREQUENCY + ARRAY FORMULA?), SKEW and KURT
>   * Lesson 3.2 - The Gaussian model
>     * A learning objective: Displaying the Gaussian distribution using the function NORMDIST.
>     * Description: You’ll be introduced to the Gaussian model. First, we’ll provide the theory behind, and then we’ll show some applications in spreadsheets and introduce some functions (NORMDIST,...). 
>     * Some functions introduced/used: NORMDIST
>   * Lesson 3.3 - Visual comparison of the distributions
>     * A learning objective: Superimpose the Gaussian curve on the histogram of stock returns in order to (visually) identify if returns fulfill the Gaussian assumption.
>     * Description: Start with the logic behind the process: the comparison of two distributions. This is possible by comparing the distribution of historical returns with a hypothetical Gaussian model in which the mean is the mean of average return, and the standard deviation is the standard deviation of the returns By looking how close (or how far) are one another, we can draw relevant information about the stock return distribution.
>     * Some functions introduced/used: NORMDIST
>   * Lesson 3.4 - Flaws in the Gaussian model
>     * A learning objective: Understand possible flaws/shortcomings related to the usage of the Gaussian model when modeling stock returns.
>     * Description: In this lesson, which will be mainly theoretical, we’ll make some considerations about the Gaussian model. We’ll discuss both the sides of the coin. First, we’ll explain why such a distribution is so popular; then, we’ll highlight what are the proven flaws that this distribution has when it is used to model stock returns.
>     * Some functions introduced/used: NORMINV

> Chapter 4 - Benchmarking performance
> In this final chapter, you’ll benchmark ABC stock against a market index and verify whether ABC outperformed the benchmark or not. The comparison process will be done through several steps/metrics. First, you’ll analyze the only cumulative returns. Next, you’ll extend the comparison using different indicators such as Sharpe Ratio and Drawdown. Finally, you’ll examine the linear relation between ABC stock and the benchmark through the correlation coefficient. At the end of the chapter, you’ll be introduced to more powerful and advanced spreadsheet features that introduce the interactivity feature in your analysis.
>   * Lesson 4.1 - Cumulative returns comparison
>     * A learning objective: Compare the performance of the ABC stock with a benchmark through a cumulative returns graph.
>     * Description: You’ll learn how to generate a cumulative return graph reporting the returns realized on both the ABC stock and the market index during the period under analysis.
>     * Some functions introduced/used: + and * operators.
>   * Lesson 4.2 - Performance metrics comparison
>     * A learning objective: Compare and rank different investments using indicators such as the Sharpe ratio and the Maximum Drawdown.
>     * Description: We’ll extend the comparison by using indicators (such as the Sharpe Ratio, the Sortino Ratio, and the Maximum Drawdown) that allow ranking different investments. 
>     * Some functions introduced/used: MAX, MIN, AVERAGE, STDEV (unbiased)
>   * Lesson 4.3 - Correlation analysis
>     * A learning objective: Assess the linear dependence between two securities through the Pearson Correlation coefficient. 
>     * Description: The learner will be introduced to the concept of historical correlation, an indicator which measures the linear dependence between two set of historical returns.
>     * Some functions introduced/used: CORREL
>   * Lesson 4.4 - Making it interactive!
>     * A learning objective: Make the application interactive to the user.
>     * Description: Maybe here just a video to show how to select a stock when several stocks are available. Same for the benchmark. Then we can extend to a particular time period.
>     * Some functions introduced/used: List selection, IF, VLOOKUP
  
  - [ ] Does each lesson have a clear learning objective?
  - [ ] Does each lesson include a brief list of functions or packages that the student will use?
  - [ ] Does the outline have at least 12 lessons and no more than 15?
