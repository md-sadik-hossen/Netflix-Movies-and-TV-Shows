## NETFLIX Movies and TV_Shows (Summarized)
![NETFLIX](https://github.com/md-sadik-hossen/Netflix-Movies-and-TV-Shows/blob/main/images/netflix_page_cover.jpg)

### Business Problem <br>
- To analyze the data and generate insights that could help Netflix decide which type of shows/movies to produce and how they can grow the business in different countries.<br>
- To develop a movie and TV show recommendation function, users should have the capability to search for a specific movie or TV show by its name. Upon entering the title, the system should generate recommendations based on similar content. <br>

To achieve the desired solution, a recommendation system will be developed by following these steps.

1. **Data Understanding:**
  - The initial stage involves comprehending the dataset. In this project, there are 12 variables, six of which contain missing values.

2. **Univariate Exploratory Data Analysis (EDA):**
  - Conduct an in-depth analysis of individual variables within the dataset to gain insights and understand their distributions and characteristics.

3. **Data Preparation:**
  - Prepare the dataset for analysis by addressing missing values, handling categorical variables, and performing any necessary transformations or preprocessing steps.

4. **Recommendation System with Cosine Similarity:**
  - Implement a recommendation system using cosine similarity.
  - This method utilizes text similarity between titles and descriptions to recommend similar titles.
  - It involves vectorizing the text data and calculating the similarity between vectors.
  - To obtain title recommendations, select the title with the highest similarity score and retrieve the corresponding TV series or movie title along with its description.

### Top Countries with the Highest Number of Shows
![NETFLIX](https://github.com/md-sadik-hossen/Netflix-Movies-and-TV-Shows/blob/main/images/1.2%20Top%2015%20Countries%20with%20the%20Highest%20Number%20of%20Shows.png)
The USA dominates with 3689 titles, followed by India with 1046 titles.UK, Canada, and France also contribute significantly, with 804, 445, and 393 titles respectively. Asian countries like Japan and South Korea have notable contributions, with 318 and 231 titles respectively.

### Content Added Over the Year
![NETFLIX](https://github.com/md-sadik-hossen/Netflix-Movies-and-TV-Shows/blob/main/images/1.3%20Content%20Added%20Over%20the%20Year%20(After%202000).png)

The years 2018 and 2017 saw the highest number of show releases, with 1147 and 1032 respectively, indicating a peak in content production. <br>
From 2012 to 2018, It shows a rapid expansion in the entertainment industry.

### Average Movie Duration Lineplot from 1940 to 2021
![NETFLIX](https://github.com/md-sadik-hossen/Netflix-Movies-and-TV-Shows/blob/main/images/4.1%20Average%20Movie%20Duration%20Over%20Years.png)

- Movie duration varied across years, peaking in 1964 with an average of 200.5 minutes and dipping to 35 minutes in 1942.
- There's a noticeable fluctuation from 1964 to 1978, with some years experiencing longer durations than others.
- More recent years show a trend towards shorter average durations, with 2020 and 2021 having average durations of 92.1 and 96.4 minutes, respectively.

### Content Ages Distribution
![NETFLIX](https://github.com/md-sadik-hossen/Netflix-Movies-and-TV-Shows/blob/main/images/8.1%20Ages%20Distribution.png)
Among content, Adults comprise 46.54%, while Teens account for 30.09%. Older Kids and Kids constitute 16.92% and 6.45%, respectively. Recommendations may prioritize adult and teen-oriented content.

### Movies and TV Shows Added Across Each Day
![NETFLIX](https://github.com/md-sadik-hossen/Netflix-Movies-and-TV-Shows/blob/main/images/9.2%20Movies%20and%20TV%20Shows%20Added%20Across%20Each%20Day.png)
While peaks are observed on days 1 and 15, possibly indicating the beginning and middle of the month, day 2 reflects a stark drop, suggesting a possible follow-up effect.

### Word Frequency Analysis
#### Word Frequency Analysis of Netflix Description Before 2012
![NETFLIX](https://github.com/md-sadik-hossen/Netflix-Movies-and-TV-Shows/blob/main/images/10.2%20Word%20Frequency%20Analysis%20of%20Netflix%20Description%20Before%202012.png)
#### Word Frequency Analysis of Netflix Description After 2012
![NETFLIX](https://github.com/md-sadik-hossen/Netflix-Movies-and-TV-Shows/blob/main/images/10.3%20Word%20Frequency%20Analysis%20of%20Netflix%20Description%20After%202012.png)

**Common Words** <br>
**Life Theme**: "Life" emerges as the most frequent theme in Netflix movie descriptions, indicating a focus on the human condition and life's experiences.<br>
**Love and Family**: "Love" and "family" are also prevalent, highlighting the popularity of movies centered around these themes.<br>
"New" Indicates fresh or innovative content and "Find" Implies discovery or exploration within the narrative.<br>

**Unique Words**:<br>
Before 2012, "young" in Netflix content suggests a recurring theme of youth experiences, appealing to a younger audience and After 2012, "Take" Suggests a unique perspective or approach.


### Recommendation System
Various techniques are used in recommendation systems, such as Collaborative Filtering, Content-Based Filtering, and Hybrid Recommendation Systems. Each technique aims to predict or recommend products, such as movies or music, to consumers. We specifically focus on Content-Based Filtering.
**Multiple Content-Based Recommendation System**

![NETFLIX](https://github.com/md-sadik-hossen/Netflix-Movies-and-TV-Shows/blob/main/images/Recommendation%20system.JPG)

Initially, we employed the TF-IDF method. However, applying TF-IDF solely on the content descriptions yielded unexpected results. This outcome might be attributed to the nature of the content descriptions, which were primarily summaries. Had the descriptions contained more comprehensive information about each movie, I believe this method would have demonstrated better performance.

Using multiple columns in the Cosine Similarity function, we achieve the best results. By incorporating data from various columns, such as title, director, cast, country, listed_in, description, and ages, the Cosine Similarity function can generate more accurate recommendations. This approach allows for a comprehensive analysis of the content, taking into account different aspects such as genre, plot, cast members, and production details.
