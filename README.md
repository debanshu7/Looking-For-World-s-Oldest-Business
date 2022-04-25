# Looking-For-World-s-Oldest-Business
Used SQL to find World's oldest businesses formed and still running

An important part of business is planning for the future and ensuring that the company survives changing market conditions. Some businesses do this really well and last for hundreds of years. BusinessFinancing.co.uk researched the oldest company that is still in business in (almost) every country and compiled the results into a dataset. In this project, I explored that dataset to see what they found.

The database contains three tables.
First one is the category table which contains the category code and category name.
Second one is countries table containing of country code, country and continent name .
The last one is Business table having information about name, year founded, category of the business.

Step -1 
Importing the database and selecting the oldest and newest business formed within the database using min() and max() command. 

Step -2 
In one country, the oldest business was founded to be 1990 whereas in another, oldest business was founded back in 578. Now, to further simplify the database, I found the number of business where founding year was before 1000. 

Step -3 
Now we do know that there are just 6 business founded before 1000. Time to extract more information about them. 

Step - 4 
Although we know where Kongo Gumi (world’s oldest operating company) was founded, what does it do? For this we need to import data from categories table using INNER JOIN. 

Step-5 
Now it’s time to have a look at various categorizes and number of businesses registered in each category via GROUP BY () and ORDER BY() clause.
 
Step -6 
But where are these so old business located, for this we need to join businesses table to countries table
 
Step -7 
It’s time to join all 3 tables together and extract only important information from each
 

Step-8
Now as we have information about all the businesses formed, we can ask questions, for example, which are the most common categories for the oldest businesses on each continent?
 
Step-9
Combining continent and business category led to a lot of results. It's difficult to see what is important. To trim this down to a manageable size, let's restrict the results to only continent/category pairs with a high count.

CONCLUSION - 
   1) We found out that the oldest business was formed in Japan named as Kongo Gumi and it was a construction business.
   2) Oldest business registered in Asia was in 578 whereas oldest business formed in Oceania was in 1809.
   3) Africa has most old business lasting in banking and finance(17) , followed by Europe in Distillers and Breweriers(12) and then Africa in aviation and        transport(10)
 

