# Box Office Mojo Revenue Analysis

Problem:  To create a multiple linear regression model to determine which features impact box office revenue in order to predict the type of movie to make in the future.

### Data
Metrics on www.boxofficemojo.com and www.imdb.com will be used for this analysis.  Box office data from 2020 and 2021 may impact the analysis due to the pandemic shuttering theaters.

### Features and Target
The features of the data set we expect to work with are: 

- Movie Title
- Domestic Gross
- International Gross
- Budget 
- Runtime in minutes
- Genre a category of artistic composition, characterized by similarities in form, style, or subject matter. More specifically, a film genre is a motion picture category based on the narrative elements that relate to the main driving force behind the story arc. There are 30 Genres in the data set.  Action | Adult | Adventure | Animation| Biography | Comedy | Crime | Documentary | Drama| Family | Fantasy| Film Noir | Game Show | History | Horror | Musical| Music | Mystery | News | Reality-TV | Romance | Sci-Fi | Short| Sport | Talk-Show | Thriller | War | Western 
- Brand examples include Marvel Comics, Lucasfilm, Pixar, etc
- Franchise examples are Marvel Cinematic Universe, Star Wars, Jurassic Park, etc
- Earliest Release Date
- Star Rating
- Cast

The individual sample/unit of analysis in this project is one movie with the features described above.  

The target will be box office worldwide gross. 

### Model and Tools
- The requests library will be used for requesting the HTML code.  Beautiful Soup will be used to parse the HTML data and Selenium will be used as a driver for site navigation
- A linear regression model will be used to model the data  
- Matplotlib and Seaborn will be used for visualization
- At this time there are no plans to utilize additional tools beyond what has been identified  

### MVP
The MVP goal of this project is a linear regression model with one feature and its relationship to box office worldwide gross.

### Potential Additional Data Sources
-  Influencer rankings for stars

