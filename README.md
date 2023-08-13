# Q1: Popular US baby names (35 marks)
!!! VERY IMPORTANT. PLEASE READ !!!
Please DO NOT upload any data (TXT files, pdf files, .db file, etc) to GitHub for this part as the data is too large!
There are some restriction and issues if you upload files that are too large in GitHub. See here to learn more
You will lose marks if you have uploaded any of them - even if you delete them afterwards
When uploading your work via GitHub Desktop, you can select what files to upload on the left by checking (and unchecking) the boxes corresponding to the files you want to (and do not want to) upload, as demonstrated in Workshop 5
I have modified the setting for your problem set repository so that by default it should not let you upload the data/namesbystate folder, the data/namesbystate.zip, or the .db file, and you should not see them available on the left
However, if for some reason any of the data files appear on the left, you should uncheck the boxes corresponding to those files
In this question, we will use the US baby names dataset from The United States Social Security Administration to create a database and answer some questions.

Go to https://www.ssa.gov/oact/babynames/limits.html, read the Background information, download the state-specific data on baby names, save the zip file under the data folder and unzip the file in the data folder
Note:
Each TXT file should be under the data/namesbystate folder. Please DO NOT add/delete/modify any of the files
Please DO NOT upload any of the TXT files as mentioned above
[Database normalisation] Read the "readme" file in the dowloaded folder and have a look of some of the tables in the TXT files. Find out if the tables represented by the TXT files are in 1NF? 2NF? 3NF? Please explain your answer
[Manage data in database] Use the Python module sqlite3 with SQL commands, create a database and create a table containing the records from all the TXT files. Please enforce the right constraints on each attribute, including setting the primary key
Note:
The code used should be as "automatic" as possible. For example, you should NOT need to write separate code to load each of the files, or separate SQL commands to insert each line of records
Please DO NOT upload the database data (.db file) as mentioned above
[SQL query] Answer each part below using one single SQL query via sqlite3:

(a) Find out the number of baby boys and the number of baby girls born in California (CA) in each year from 2010
Do you observe any trend?
(b) List out the most popular boy names and the most popular girl names with the corresponding counts in the US in every 10 years from 1910 to 2020
Here "the most popular boy/girl name" in a given year means it is the name with the highest number of boy/girl babies born in that year in the US with that name
Your result should have 22 names and 22 counts corresponding to 1910 boy, 1920 boy, ..., 2020 boy, 1910 girl, 1920 girl, ..., 2020 girl
You can hard code all the years if you want to
For (4b), you do not need to worry if there are two names with the same number of counts in this part - giving one of the names with the highest count is sufficient
(c) List out the most popular baby names and corresponding counts in each state in 2020, order the counts in descending order
In order words, for each state, provide the baby name(s) that has the highest number of babies born in 2020 with that name, and the corresponding number of babies born in 2020 with that name)
Please make sure all query results are shown in the notebook. You SHOULD NOT make use of any SQL command / keywords that we did not cover in the course.

Note:

Each part should be answered by using one SQL query only

A query involving subquery counts as one query
The result from the SQL query should answer the corresponding part directly and should NOT require any further cleaning or effort. For example:

You should NOT make use of Python functionality like loops, slicing, Pandas functionality, etc
It should NOT involve eyeballing the answer
Except for the question "Do you observe any trend?"
It should NOT involve hard coding of values except those mentioned in the questions
For example, it is okay to hard code 2020 for part (c) as 2020 is mentioned in the question, but if you hard code the maximum count for part (c) you will lose marks as it should be found via SQL query
If you cannot use one query to answer the question, you can answer with a few queries with some hard coding

But of course you will lose some points
Please state the assumptions that you have made when answering the questions
