# Sakila DVD Rental database Analysis
PDSND - Udacity Project One:  Investigating a Relational Database
 

## Introduction

The Sakila Database holds information about a company that rents movie DVDs. In this project, the Sakila DVD Rental database was queried to gain an understanding of the customer base, such as what the patterns in movie watching are across different customer groups, how they compare on payment earnings, and how the stores compare in their performance. For assistance in the queries, the schema for the DVD Rental database was used as given in the `dvd-rental-erd.pdf`.


## Local Environment Setup 
To analyze the data, **PostgreSQL** was installed on the local machine.

For detailed instructions on how to install  PostgreSQL, vist 
http://www.postgresqltutorial.com/install-postgresql/


Once PostgreSQL server is installed, we need to download the Movie database from: [PostgreSQL Sample Database](http://www.postgresqltutorial.com/postgresql-sample-database/)


To load the DVD Rental database into our PostgreSQL server on the local machine, it is recommeded to use the **PgAdmin tool**.Instructions on how to do this are available at: [Load PostgreSQL Sample Database](http://www.postgresqltutorial.com/load-postgresql-sample-database/).



## Questions worked upon for analysis

**Question 1**

We want to understand more about the movies that families are watching. The following categories are considered family movies: Animation, Children, Classics, Comedy, Family and Music.

**Create a query that lists each movie, the film category it is classified in, and the number of times it has been rented out.**

**Question 2**

Now we need to know how the length of rental duration of these family-friendly movies compares to the duration that all movies are rented for. **Can you provide a table with the movie titles and divide them into 4 levels (first_quarter, second_quarter, third_quarter, and final_quarter) based on the quartiles (25%, 50%, 75%) of the rental duration for movies across all categories?** Make sure to also indicate the category that these family-friendly movies fall into.

**Question 3**

Finally, provide a table with the family-friendly film category, each of the quartiles, and the corresponding count of movies within each combination of film category for each corresponding rental duration category. The resulting table should have three columns:

- Category
- Rental length category
- Count

**Question 4**

We want to find out how the two stores compare in their count of rental orders during every month for all the years we have data for. **Write a query that returns the store ID for the store, the year and month and the number of rental orders each store has fulfilled for that month.**
Your table should include a column for each of the following: year, month, store ID and count of rental orders fulfilled during that month.
**The count of rental orders is sorted in descending order.** 