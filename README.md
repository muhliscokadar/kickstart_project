# KickStart Chart

## Background

Over two billion dollars have been raised using the massively successful crowdfunding service, Kickstarter, but not every project has found success. Of the over 300,000 projects launched on Kickstarter, only a third have made it through the funding process with a positive outcome.

Since getting funded on Kickstarter requires meeting or exceeding the project's initial goal, many organizations spend months looking through past projects in an attempt to discover some trick to finding success. 

The Goal: Organize and analyze a database of four thousand past projects in order to uncover any hidden trends.

## Instructions

## Kickstarter Table

* Using the Excel table provided, modify and analyze the data of four thousand past Kickstarter projects as you attempt to uncover some of the market trends.

* Used conditional formatting to fill each cell in the `state` column with a different color, depending on whether the associated campaign was "successful," "failed," "cancelled," or is currently "live".

* Created a new column at column O called `percent funded` that uses a formula to uncover how much money a campaign made towards reaching its initial goal.

  * Used conditional formatting to fill each cell in the `percent funded` column using a three-color scale. The scale should start at 0 and be a dark shade of red, transitioning to green at 100, and then moving towards blue at 200.

* Created a new column at column P called `average donation` that uses a formula to uncover how much each backer for the project paid on average.

* Created two new columns, one called `category` at Q and another called `sub-category` at R, which use formulas to split the `Category and Sub-Category` column into two parts.

  ## Category Stats

  * Created a new sheet with a pivot table that will analyze your initial worksheet to count how many campaigns were "successful," "failed," "cancelled," or are currently "live" per **category**.

    * Created a stacked column pivot chart that can be filtered by `country` based on the table that was created.

  ## Subcategory Stats

  * Created a new sheet with a pivot table that will analyze your initial sheet to count how many campaigns were "successful," "failed," "cancelled," or are currently "live" per **sub-category**.

    * Created a stacked column pivot chart that can be filtered by `country` and `parent-category` based on the table you have created.

* The dates stored within the `deadline` and `launched_at` columns are using unix timestamps.

  * Created a new column named Date Created Conversion that used to convert the data contained within launched_at into Excel's Date format

  * Created a new column named Date Ended Conversion that used to convert the data contained within deadline into Excel's Date format

  ## Outcomes Based on Launch Date

  * Created a new sheet with a pivot table with a column of `state`, rows of `Date Created Conversion`, values based on the count of `state`, and filters based on `parent category` and `Years`.

  * Created a pivot chart line graph that visualizes this new table.

* Creatd a report in Microsoft Word and answer the following questions...

1. What are three conclusions we can make about Kickstarter campaigns given the provided data?
2. What are some of the limitations of this dataset?
3. What are some other possible tables/graphs that we could create?

## Advanced

* Created a new sheet with 8 columns: `Goal`, `Number Successful`, `Number Failed`, `Number Canceled`, `Total Projects`, `Percentage Successful`, `Percentage Failed`, and `Percentage Canceled`

  * In the `goal` column, create twelve rows with the following headers...

    * Less Than 1000
    * 1000 to 4999
    * 5000 to 9999
    * 10000 to 14999
    * 15000 to 19999
    * 20000 to 24999
    * 25000 to 29999
    * 30000 to 34999
    * 35000 to 39999
    * 40000 to 44999
    * 45000 to 49999
    * Greater than or equal to 50000

## Goal Outcomes


  * Used the `COUNTIFS()` formula, count how many successful, failed, and canceled projects were created with goals within those ranges listed above. Populate the `Number Successful`, `Number Failed`, and `Number Canceled` columns with this data.

  * Added up each of the values in the `Number Successful`, `Number Failed`, and `Number Canceled` columns to populate the `Total Projects` column. Then, using a mathematic formulae, find the percentage of projects which were successful, failed, or were canceled per goal range.

  * Created a line chart which graphs the relationship between a goal's amount and its chances at success, failure, or cancellation.

## Observations

# 1. What are three conclusions we can make about Kickstarter campaigns given the provided data?

* Top three categories are Theater 839, Music 540, and Film & Video 520 based on a total of a successful project in descending order.

* Top three categories are Music 77%, Theater 60%, and Film & Video 58% based on a percentage of successful (number of the total project by successful project) in descending order.

* Technology, Publishing, Food are least successful categories if we ignore the journalism.
    
    * Based on these outcomes, Theater, Film & Music which are in entertainment category seems more successful which does not require technical skills in performing. We could say that these fields are more popular among people.

    * In other hands, technology, food, publishing categories need more technical skills that require more expertise in this field and they are least successful categories.

    * There is a negative rate of change between Goal (in dollars) and successful rate. It is decreasing.

    * Almost 71% of the project who kept their goal below $1000 were successful.

# 2. What are some of the limitations of this dataset?

* If we are looking what is the recipe to have a successful campaign based on this data, it is hard to make predictions if a project will be successful or not. The only information can be gathered from this data is what categories and sub-categories were more successful, failed, canceled or live based on the country and pledged donations with the start and end date of the campaign.

* A successful campaign cannot be determined from this data set. In order to predict if a project that will be successful or not, maybe there could be another data set that may provide more insights of successful campaigns only.

# 3. What are some other possible tables/graphs that we could create?

* A table/graph of which category or sub-category got a higher donation.

    * For example, there were 444 projects for over 50000 Goal and only 19% of them got successful.

* A table/graph of categories based on the pledged donations.

* A graph of each category based on their countries.

* A graph of each category based on their countries and outcomes.




