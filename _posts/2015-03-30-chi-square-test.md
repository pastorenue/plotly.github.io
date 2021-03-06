---
layout: two_column_layout
title: Chi-Square Test
subtitle: A Step by Step Guide to the Chi-Square Test
permalink: /chi-square-test
imageurl: /static/images/chi-square/thum-chi-square.png
state: active
tags: classroom statistical
meta_description: A step by step tutorial on Chi-Square tests. Make a graph online and for free with Plotly
---

#Chi-Square Test

<div>
    <a href="https://plot.ly/~jackp/4102/" target="_blank" title="$\text{Probability density function of } \chi^2_k$" style="display: block; text-align: center;"><img src="https://plot.ly/~jackp/4102.png" alt="$\text{Probability density function of } \chi^2_k$" style="max-width: 100%;width: 800px;"  width="800" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="jackp:4102" src="https://plot.ly/embed.js" async></script>
</div>

The chi-squared test is a statistical hypothesis test that provides a quantitative method to compare observed frequencies with expected frequencies. For example, we could use a chi-squared test to evaluate if a coin is likely biased or to determine if elevated cholesterol is related to gender.

The general strategy to perform a chi-squared test is to calculate the chi-squared value (or chi-squared statistic), and then use a table of chi-squared values to estimate the probability that our result is due to chance alone. This probability is called the p-value. The null hypothesis, i.e., that the difference between expected and observed frequencies isn’t significant, is typically accepted for p-values greater than .05.

In 2012, Gallup determined that [5% of Americans consider themselves vegetarians](http://www.gallup.com/poll/156215/consider-themselves-vegetarians.aspx). Their study was based on a telephone survey of 1014 adults (506 women and 508 men). Note that the data we’re using here is based on percentages reported. We’ll use a chi-squared test to decide if vegetarianism can be correlated to gender.

Here’s how to use Plotly to calculate both the chi-squared statistic and the p-value for you.

###Step 1 : Set up the grid

We’ve already entered the [Gallup poll data into Plotly](https://plot.ly/976/~mariahh). Click the link to open the data in your workspace. | ![Chi square test](/static/images/chi-square/01-chi-square.png)

###Step 2: Chi-squared test

Once the data has opened in your workspace, select <strong>Chi-squared test</strong> from the ANALYSIS menu. | ![Chi square tes](/static/images/chi-square/02-chi-square.png)

Because we want to compare the sample data with what we would expect assuming no gender bias, we select “choose as obs” in the Vegetarian column and “choose as exp” in the Expected vegetarian column. Next, click on **Perform Chi-squared Test**. | ![Chi square tes](/static/images/chi-square/03-chi-square.png)

Plotly puts our results in the first two columns to the right of our data. In this case, the chi-squared statistic is 4.1456 and the P-value is 0.04174. By convention, because 0.04174 is less than 0.05, we decide that the difference is statistically significant. In other words, we reject the null hypothesis and conclude that there must be a relation between vegetarianism and gender. | ![Chi square tes](/static/images/chi-square/04-chi-square.png)
