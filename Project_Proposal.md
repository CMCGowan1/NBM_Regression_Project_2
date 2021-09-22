# Box Office Mojo Revenue Analysis

A movie producer has engaged CMCAnalytics, AKA Cheryl McGowan, to complete a data science project to figure out how to maximize future movie box office revenue.  The client is specifically interested in which genres the movie going public is interested in seeing. Can we predict what movie genre will produce the most daily revenue at the box office?  The movie producer will use this information to guide decision making on which movies to produce in the coming years for their company. Additional insight may be available on which brands or franchises to partner with in order to bring new movies to market and what day of the week is most impactful to release a certain genre.

### Data
Metrics on www.boxofficemojo.com will be used for this analysis.  Data will be scraped using Beautiful Soup and Selenium.  Data from 2020 and 2021 will not be used due to the pandemic shuttering theaters.

### Features and Target
The features of the data set we expect to work with are: genre, brand, franchise, country of origin, budget, lifetime gross, release date, number of dats since original release date, daily box office revenue, day of the week and movie title. 

- Genre is a category of artistic composition, characterized by similarities in form, style, or subject matter. More specifically, a film genre is a motion picture category based on the narrative elements that relate to the main driving force behind the story arc. There are 30 Genres in the data set.  
  - Action | Adult | Adventure | Animation| Biography | Comedy | Crime | Documentary | Drama| Family | Fantasy| Film Noir | Game Show | History | Horror | Musical| Music | Mystery | News | Reality-TV | Romance | Sci-Fi | Short| Sport | Talk-Show | Thriller | War | Western 

- Brand examples include Marvel Comics, Lucasfilm, Pixar, etc
- Franchise examples are Marvel Cinematic Universe, Star Wars, Jurassic Park, etc
- Country of Origin  
- Budget 
- Lifetime Gross  
- Release Date of original release, not re-release
- Numbers of Days Since Release Date calculated from Original Release Date and end date of December 31, 2019.
- Daily Box Office
- Day of the Week: MTWTFSS
- Movie Title
- Ave Daily Revenue for total days released - like per square foot sales


A subset of the features will be the individual sample/unit of analysis in this project.  TBD based on an iterative process using Linear Regression modeling to find the feature or features that best fit the model.

## Target
The target will be daily box office revenue. 

### Model and Tools
- Beautiful soup and Selenium will be used for webscraping.  Beautiful Soup will be used to parse the HTML data and Selenium will be used as a driver for site navigation
- A linear regression model will be used to model the data  
- Matplotlib and Seaborn will be used for visualization
- At this time there are no plans to utilize additional tools beyond what has been identified  

### MVP
The MVP goal of this project is a linear regression model with one feature genre and its relationship to daily box office revenue.

### Potential Additional Data Sources
-  Popular news stories 
-  Top Book Genres 
-  Pulitzer prize willing books
-  Oprahs book club 
-  Popular TV genres
-  IMDbPro Free trial may have additional data points

