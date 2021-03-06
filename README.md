# Microsoft Theater's Debut Film

##### Contributors:
##### - James Shaw, shawjr3@gmail.com
##### - Nick Pardue, nickpardue@gmail.com

### [Our Presentation]

![microsoft_theater.png](https://github.com/godelayheehoo/Nick-and-James-mod-1-project/blob/branchy/Images/microsoft_theater.png)

### Our Business Problem
Microsoft is launching a movie studio in an effort to start producing content in the film industry (a $136 billion industry as of 2018). We were tasked with doing data analysis and creating a presentation to explore what types of films are currently doing the best at the box office, and provide actionable insight for the purposes of deciding what type of film they should create. 

As many would love to see a company like Microsoft fail, we wanted to look at variables that would lead to a "safe" debut production. We defined "safe" as a movie that would have a high profit percent with a firm confidence interval.

We chose to use movie data sourced from [IMDb] and [The Numbers]. Using this data, we sought to find out the following:
- Are there any months in which movies released tend to make the most profit?
- Which genre(s) are most profitable?
- Are there any writers that will increase our odds at creating a successful movie?

### Data Sets
Our Sourced Data
- [Budgets and Release Dates]
- [IMDb Title Codes and Genres]
- [Writer IMDb Codes and Title Codes]
- [Writer Names]

[Our Cleaned Data] 


### Cleaned Data Description
We analyzed a dataset of 1,348 movies, each containing the following *relevant* variables:
 - title
 - tconst
    - A variable IMDb uses to identify the title of each movie.
 - release_year
     - Ranging from 2000 - 2019
 - month
 - genres
    - Any genre that appeared on at least 95 entries.
 - writers
 - experienced_writers 
    - Any writer with at least three (3) entries.
 - profit_percent
    - A function showing net profit in relation to production budget.
 

### Exploratory Analysis

 ##### Figure 1: Overall Percent Profit by Month
 - July was found to have the highest mean profit percent (191.96%), with a 95% confidence interval of (152.38%, 231.54%). 
 
![pp_by_month.png](https://github.com/godelayheehoo/Nick-and-James-mod-1-project/blob/branchy/Images/pp_by_month.png)

 ##### Figure 2: Each Genre's Average Profitability in July
 - Animation was found to have the highest mean percent profit in July at 359.99%, compared to the average across all genres of 161.43%. 
 
![genres_in_july.png](https://github.com/godelayheehoo/Nick-and-James-mod-1-project/blob/branchy/Images/genres_in_july.png)

 ##### Figure 3: Animation's Profitability in July
 - We plotted each genre's percent profit by month. Featured below is Animation's. As mentioned above, the mean was 359.99%, with a 95% CI of (211.99%, 507.99%).
 
![animation_pp_by_month.png](https://github.com/godelayheehoo/Nick-and-James-mod-1-project/blob/branchy/Images/animation_pp_by_month.png)

 ##### Figure 4: Animation's Most Profitable Writers
 - We looked at experienced writers within the Animation genre, finding their average percent profit to be 354.59%. This was higher than the average percent profit of all experienced writers (288.63%), and even higher still than that of the average animation writer (219.34%).

![writers_animation.png](https://github.com/godelayheehoo/Nick-and-James-mod-1-project/blob/branchy/Images/writers_animation.png)

### Limitations
- Can't control how large Hollywood has blown up internationally in recent times, even with trimming our data to exclude movies released prior to 2000.
- Did not control for time spent in theaters.
- We had no way of excluding movies released online (e.g. Netflix movies).
- Hollywood accounting. There are no *free* ways of getting:
    - Non-user-reported gross sales
    - Advertising budget for domestic or foreign marketing
- Effects of international markets on gross sales.

### Future Improvements
- Compile a larger dataset.
- Expand initial grouping to a seasonal format, rather than by month.
- Explore what production costs provide the highest percent profit.
- Look into the impact experienced directors have on percent profit.
- Investigate how a movie's opening weekend affects gross sales.

### Reproducing Our Data
Please visit the Appendix in our [Technical Notebook].

### Repo Navigation
```
├── Images
│   ├── .DS_Store
│   ├── animation_pp_by_month.png
│   ├── genres_in_july.png
│   ├── microsoft_theater.png
│   ├── pp_by_month.png
│   └── writers_animation.png
│
├── .gitignore
│
├── Browser Friendly Technical Notebook.html
│
├── Microsoft New Studio Recommendations - Technical Notebook.ipynb
│
├── Proposal.pdf
│
├── README.md
│
├── data_for_initial_load.csv
├── imdb.name.basics.csv.gz
├── imdb.title.basics.csv.gz
├── imdb.title.crew.csv.gz
└── tn.movie_budgets.csv.gz

```

### Sources of Images Used in Proposal
- Slide 1: https://www.microsofttheater.com/news/detail/la-lives-home-of-concerts-and-award-shows-renamed-microsoft-theater
- Slide 2: https://www.visitlasvegas.com/listing/buffalo-bills-movie-theater/36671/
- Slide 10: https://www.mycustomer.com/experience/engagement/understanding-customer-journeys-the-four-limitations-of-traditional-analytics
- Slide 11: https://www.odysys.com/blog/research-blogging-ideas/


[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [our presentation]: <https://github.com/godelayheehoo/Nick-and-James-mod-1-project/blob/master/Proposal.pdf>
   [the numbers]: <https://www.the-numbers.com/>
   [themoviedb]: <https://www.themoviedb.org/?language=en-US>
   [imdb]: <https://www.imdb.com/?ref_=nv_home>
   [our cleaned data]: <https://github.com/godelayheehoo/Nick-and-James-mod-1-project/blob/master/data_for_initial_load.csv>
   [our sourced data]: <https://github.com/godelayheehoo/Nick-and-James-mod-1-project/tree/branchy/Data/Sourced%20Data>
   [budgets and release dates]: <https://github.com/godelayheehoo/Nick-and-James-mod-1-project/blob/master/tn.movie_budgets.csv.gz>
   [imdb title codes and genres]: <https://github.com/godelayheehoo/Nick-and-James-mod-1-project/blob/master/imdb.title.basics.csv.gz>
   [writer imdb codes and title codes]: <https://github.com/godelayheehoo/Nick-and-James-mod-1-project/blob/master/imdb.title.crew.csv.gz>
   [writer names]: <https://github.com/godelayheehoo/Nick-and-James-mod-1-project/blob/master/imdb.name.basics.csv.gz>
   [technical notebook]: <https://github.com/godelayheehoo/Nick-and-James-mod-1-project/blob/master/Microsoft%20New%20Studio%20Recommendations%20-%20Technical%20Notebook.ipynb>



