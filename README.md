# Surfs_Up
On my vacation in Hawaii last year, I discovered a new found passion for surfing. I have been trying to come up with a plan that will not only let me return to Hawaii but live there forever.  I finally come up with an idea that I think is interesting, a surf 'n' shake shop, serving surf boards and icecream to locals as well as travelers. I have some savings that I ma willing to invest but I would be needing some real investor backing to get this off the ground.  After putting together a strong business plan I reach out to an investor named W Avy. 

## Purpose: 
The purpose of this analysis is to provide more information about temperature trends before opening the surf shop in Oahu. This analysis provides temperature data for the months of June and December in Oahu, Hawaii in order to determine if the surf and ice cream shop business would be sustainable year-round.

## Background:
The meeting with the investor W. Avy goes extremely well but he has a concern about the weather. He is extremely serious about this. He has invested in a surf shop earlier in his career. However, he did not ask for any weather analysis and that early venture failed.
W. Avy likes the analysis, but he wants more information about temperature trends before opening the surf shop. Specifically, he wants temperature data for the months of June and December in Oahu, in order to determine if the surf and ice cream shop business is sustainable year-round.

## Tasks:
W. Avy is concerned about the amount of precipitation on Oahu. There needs to be enough rain to keep everything green, but not so much that you lose out on that ideal surfing and ice cream weather. I  know that I can set W. Avy's mind at ease by analyzing precipitation levels and showing him the cold, hard, data that backs up Oahu as the perfect place to surf. I  have the last 12 months of precipitation data already loaded into your SQLite database, so we are ready to go. W. Avy supplied me with the data he wants us to use and has asked me to look at a full year of data. 

This project consists of the following two technical analysis deliverables and a written report:

- Deliverable 1: Determine the Summary Statistics for June - Using Python, Pandas functions and methods, and SQLAlchemy, we will filter the date column of the Measurements table in the hawaii.sqlite database to retrieve all the temperatures for the month of June. We will then convert those temperatures to a list, create a DataFrame from the list, and generate the summary statistics.

- Deliverable 2: Determine the Summary Statistics for December - Using Python, Pandas functions and methods, and SQLAlchemy, we will filter the date column of the Measurements table in the hawaii.sqlite database to retrieve all the temperatures for the month of December. We will then convert those temperatures to a list, create a DataFrame from the list, and generate the summary statistics.

- Deliverable 3: A written report for the statistical analysis (README.md) - The Readme.md file will discuss the details of the project and provide an analysis, overview and a summary of the tasks completed in the project.


## Tools Used:
- 1. SQLite 
- 2. Python 3.9, 
- 3. Visual Studio Code 1.50.0, 
- 4. Anaconda 4.8.5, 
- 5. Jupyter Notebook 6.1.4, 
- 6. Libraries: Pandas, Numpy, Datetime
- 7. Sqlalchemy dependency ( automap, session, create_engine, func)
- 8. Matplotlib dependencies

#### SQLite :
- Advantages - The main advantages are:

  - It's local. One of the core advantages of SQLite is that it allows you to create databases locally on your computer to support testing and easy prototyping. This is beneficial, because if you want to test something out and you need a database, it's not always the most convenient to set up a SQL database server just to try something out.

  - There's an app for that. Another advantage of SQLite databases are that they can be used on a mobile phone app. Most mobile phone games will use an SQLite database to store certain information about you or your players statistics. 

- Disadvantages - SQLite also has a couple of disadvantages, however. They are:

  - It's local. If you've used a MYSQL database before, you might have noticed that you can have multiple users access the database. With SQLite, there are no users. SQL is local: stored on one computer or phone. So, only that computer or phone will have access.

  - There are fewer security features: one other disadvantage to be aware of is that SQLite doesn't have as many security features as a traditional SQL database.

#### SQLAlchemy ORM:
One of the primary features of SQLAlchemy is the Object Relational Mapper, which is commonly referred to as ORM. ORM allows you to create classes in your code that can be mapped to specific tables in a given database. This allows us to create a special type of system called a decoupled system.

#### SQLAlchemy Create Engine:

Another really great feature of SQLAlchemy is the create engine function. This function's primary purpose is to set up the ability to query a SQLite database. After all, data just sitting in a database that we can't access does us no good. In order to connect to our SQLite database, we need to use the create_engine() function. This function doesn't actually connect to our database; it just prepares the database file to be connected to later on.

#### SQLAlchemy Automap Base:
Automap Base creates a base class for an automap schema in SQLAlchemy. Basically, it sets up a foundation for us to build on in SQLAlchemy, and by adding it to our code, it will help the rest of our code to function properly.


## Code:
- Snapshots from our code in Jupyter notebook for Deliverable 1 is shown below:


![11](https://user-images.githubusercontent.com/23488019/146658500-32450cde-7cd7-4dd6-9b77-7760b0d7d10e.PNG)


![12](https://user-images.githubusercontent.com/23488019/146658501-4538b1e6-3750-463e-be77-349026ee574c.PNG)


![13](https://user-images.githubusercontent.com/23488019/146658503-6caaba7a-89a6-4960-a2e8-639f4faf8698.PNG)



- Snapshots from our code in Jupyter notebook for Deliverable 2 is shown below:


![21](https://user-images.githubusercontent.com/23488019/146658504-f45af70f-5cf7-4535-9d3f-7c99061ccdb6.PNG)


![22](https://user-images.githubusercontent.com/23488019/146658505-99726016-56d4-467f-af78-06b3c82c804e.PNG)



## Results:

##### Deliverable 1: Summary Statistics for June -
We used the  Python function df.describe() to get the compound information about temperature for the month of June. There were total amount of 1700 records of temperature for June. The average temperature(mean) is 74.9°F. The highest temperature is 85°F and the minimum is 64°F. The function df.describe() function also gave us records for std, 25%, 50% and 75%. The tabulated result can be seen below:

![2](https://user-images.githubusercontent.com/23488019/146658208-9568974f-ab01-4315-b5ff-1bb7f4f4f5cd.PNG)


##### Deliverable 2: Summary Statistics for December -

We used the  Python function df.describe() to get the compound information about temperature for the month of December. There were total amount of 1517 records of temperature for December. The average temperature(mean) is 71.04°F. The highest temperature is 83°F and the minimum is 56°F. The function df.describe() function also gave us records for std, 25%, 50% and 75%. The tabulated result can be seen below:

![1](https://user-images.githubusercontent.com/23488019/146658234-abc362b0-4332-4a98-899e-7d7b23ab7d5b.PNG)


Our Analysis helped in a detailed The three key differences in weather between June and December is discussed below:

- 1. There is not a major differenvce between the overall temperatures between month of june and December. For the month of June it was 74.9 F and for December it was 71 F.

- 2. There was not a major difference between the maximum temperatures for both the months. It was 85 F for June and 83 F for December.

- 3. There was a major difference in th eminimum temperatures for both the months. It was 64 F for June and 56 F for December.


## Summary:

Our analysis shows that Weather in Oahu perfectly suits our surfing & ice cream shop. The temperature and precipitation outcomes show that Oahu is an ideal location year-round for the Surf and Shake shop. Since there is not a major difference in the temperatures year round, It will be a good idea to go ahead with the planning for the new shop. However, additional analysis for the rest of the months is required to confirm the temperature and precipitation for the year. Other factors such as wind level, equipment, raw materials as well as hiring of local employees can play a part in determining the cost effectiveness of the business.  

Two additional queries were performed to get a detailed insight into our analysis. These queries are discussed below:
- 1. Precipitation details for June:
We calculated the precipitation for the month of June and the code can be found below. After running the query we found the following results:

![3](https://user-images.githubusercontent.com/23488019/146658040-e61f8afe-385e-42d1-9bd7-53df96384588.PNG)


Hence it can be concluded that, th eprecipitation count fo rthe month of June was 1574 and the mean was 0.136360.

- 2. Precipitation details for December:
We calculated the precipitation for the month of December and the code can be found below. After running the query we found the following results:

![4](https://user-images.githubusercontent.com/23488019/146658044-a9e065da-375f-4b36-92ae-962465f330af.PNG)


Hence it can be concluded that the precipitation count for th emonth of December was 1405 and th emean was 0.216819.



## Resources:
- Data Source: SurfsUp_Challenge_starter_code.ipynb 
- Data File: hawaii.sqlite
- https://courses.bootcampspot.com/courses/791/pages/9-dot-0-1-exploring-weather-data?module_item_id=301370

## References:
- https://docs.python.org/3.6/library/stdtypes.html#numeric-types-int-float-complex


