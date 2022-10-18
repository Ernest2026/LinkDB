# LinkDB: A comprehensive dataset of public LinkedIn members and companies

![Illustration image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/55a33zvdklut30fr5pbq.png)

Are you aware of how easy it is to automate sales/marketing prospecting and investment analysis on LinkedIn? What if you realized that LinkDB even makes it easier?

LinkDB is an exhaustive dataset of publicly accessible LinkedIn members and companies. The database contains the profiles of 17+M companies worldwide and people’s profiles separated by regions. The regions include countries like the United States, Canada, the United Kingdom, Israel, Singapore, Australia, New Zealand, and Ireland. It also has snapshots of other countries too. You can reach out to them to get a breakdown of our people profiles by country.

To access the database you need a basic knowledge of SQL, JSON query functions and operators, and SQL/JSON path expressions. Here is a basic example of how to search users by name.

```sql
SELECT
  id,
  parsed_data->>'first_name' AS first_name, 
  parsed_data->>'last_name' AS last_name
  FROM profile
  LIMIT 10;
  ```
  
Visit their documentation if you are interested in finding out more about their search queries, e.g. finding all Apple employees or finding Software Engineers in San Francisco.

Find out more about [LinkDB](https://nubela.co/blog/linkdb-an-exhaustive-dataset-of-linkedin-members-and-companies/) in this post.

