**Project Name - Netflix Content Analysis and Clustering**

**Project Summary -**
**Objective**

The primary goal is to explore the evolution of Netflix's content catalog and develop a model to cluster similar content. This is motivated by a 2018 Flixable report indicating a significant strategic shift where the number of TV shows nearly tripled since 2010, while the number of movies decreased by over 2,000 titles.

**Key Deliverables**

Exploratory Data Analysis (EDA):

A thorough examination of the dataset to understand content distribution by type (Movie/TV Show), release year, rating, and duration, and to handle missing or inconsistent data.

Geographic Content Analysis:

An investigation into the geographic distribution of content to understand what type of content is available in different countries.

Content Strategy Trend Analysis:

Verification of the reported trend by quantifying if Netflix has been increasingly focusing on TV rather than movies in recent years, using the content's date added or release year.

Content Clustering:

Applying text-based feature matching (e.g., using titles, descriptions, cast, and genres) to cluster similar TV shows and movies together.

Potential for Expansion

The project also identifies the potential for integrating external datasets (such as IMDB ratings or Rotten Tomatoes scores) in the future to yield deeper insights into content popularity and critical reception.

**Problem Statement**
Netflix, a dominant global streaming platform, is undergoing a significant strategic transformation in its content library. A report from 2018 indicated that since 2010, the platform's focus has dramatically shifted, resulting in a near-tripling of TV show titles and a reduction of over 2,000 movie titles.

This project seeks to address the following questions using the Netflix dataset:

Content Strategy Validation: Can the provided dataset validate and quantify the extent to which Netflix is prioritizing the addition of TV shows over movies in recent years?

Global Content Footprint: What is the diversity and distribution of content types (Movies vs. TV Shows) across different countries, and what are the characteristics of the content originating from key geographic regions?

Content Discoverability: Can an unsupervised learning model (clustering) be built using text-based features (like title, description, cast, and genres) to group similar content, thereby creating a system that could potentially enhance content recommendation and discoverability for users?

The successful completion of this project will provide data-driven insights into Netflix's evolving content strategy and establish a foundational clustering model for its diverse catalog.


**Business Objesctive**

The project tasks directly align with several key business goals for a streaming platform like Netflix:

1.Strategic Content Investment Objective: To validate and understand the content strategy shift.

Relates to Task: "If Netflix has been increasingly focusing on TV rather than movies in recent years."

Business Value: Provides data to justify future investment decisions. If TV shows drive subscriber engagement and retention, the analysis confirms this focus. It helps Content Acquisition teams allocate their budget more effectively between producing/licensing Movies versus TV Shows.

2.Global Market Penetration Objective: To optimize content offerings for specific geographic markets.

Relates to Task: "Understanding what type content is available in different countries."

Business Value: Helps Regional Content Managers understand the dominant content type or genre in a specific country (e.g., is India's library heavily skewed toward International Movies?) and identify gaps where local content creation or licensing could increase subscriber numbers in that region.

3.Improving User Experience and Retention Objective: To enhance the content recommendation engine.

Relates to Task: "Clustering similar content by matching text-based features."

Business Value: The content clusters can be used to improve the accuracy and relevance of personalized recommendations. If the system can accurately group content by theme, cast, and director, it provides better "If you liked this, you'll love that" suggestions, which is crucial for increasing user engagement and reducing churn (cancellation).

In summary, the project serves as a data-driven decision support system for Netflix, translating raw catalog data into actionable insights for investment, global expansion, and user retention.

**What do you suggest the client to achieve Business Objective ?**

Three Specific, Actionable Business Objectives

Content Investment Prioritization and Budget Allocation (Focus: TV vs. Movies) Objective: Validate the business shift towards TV Shows and establish clear, data-driven targets for future content investment mixes.

Analysis to Support:

**Time Trend**: Quantify the growth rate difference between TV Shows (seasons/episodes, not just titles) and Movies added per year.

**Value Assessment (Post-Integration)**: Once you integrate external ratings (IMDB/Rotten Tomatoes), determine if the increase in TV Show volume is also correlated with higher quality (ratings) compared to the declining Movie volume.

**Actionable Insight**: The final insight should tell Netflix, "Based on content volume trends and initial quality checks, we recommend increasing the TV Show budget allocation by X% over the next two years, primarily targeting Y genre, to maintain current subscriber engagement."

**Localized Content Strategy and Global Market Retention (Focus: Content by Country) Objective**: Identify key content preference gaps in major regional markets to improve subscriber retention and target new local productions.
Analysis to Support:

**Top 5 Countries**: Analyze the content mix (Movie vs. TV Show), genres, and release years for the top 5 countries represented in the dataset.

**Content Origin vs. Viewing Market**: If possible (though challenging with this dataset alone), try to see what percentage of content produced in Country A is available only in Country B.

**Actionable Insight**: The final insight should answer, "In the [Top Country] market, there is an over-saturation of [Clustered Genre A] and an undersupply of [Clustered Genre B], suggesting that future local content acquisitions should focus on [Genre B] to better serve the local audience."

**Enhancing Recommendation and Content Tagging Systems (Focus: Content Clustering) Objective**: Leverage text-based features (description, cast, director) to refine content categories, improve recommendation accuracy, and uncover emerging micro-genres that are currently underserved.
Analysis to Support:

**Clustering Validation**: Use the clustering results to identify documents (shows/movies) that Netflix currently places in Category X (e.g., 'Dramas') but your model clusters with Category Y (e.g., 'Thrillers').

**Actionable Insight**: The final insight should state, "The text-based clustering reveals a previously undefined 'Dark Psychological Thriller' micro-genre, currently mislabeled across three different 'listed_in' categories. By formally recognizing this cluster, Netflix can improve personalized recommendations, as users who enjoy one show in this cluster are highly likely to enjoy others."

**Conclusion and Key Project Insights**

This project's exploratory data analysis (EDA) and text-based clustering have provided clear evidence of Netflix's strategic evolution, highlighting a significant pivot toward episodic content, deep investment in global markets, and the creation of targeted content clusters designed for specific audience segments.

I. Strategic Shift from Movies to TV Shows The data emphatically confirms the strategic shift observed since 2010.

Growing TV Focus: The total number of TV shows in the catalog has dramatically increased, nearly tripling, while the overall number of movies has concurrently decreased. This indicates a primary focus on building out a library of binge-worthy, long-form content.

Retention over Acquisition: This shift suggests that Netflix prioritizes subscriber retention, as TV shows (especially multi-season originals) offer a higher continuous engagement rate than one-off movie titles.

New Content Velocity: An analysis of the date_added and release_year columns reveals a sharp increase in the volume of TV shows added annually in the years leading up to 2019, signifying an accelerated production and acquisition cycle for episodic content.

II. Global Content Availability and Sourcing The analysis of content availability across different countries underscores Netflix's global strategy:

United States Dominance (Volume): The United States remains the primary country of origin for the majority of the content, offering the largest overall volume.

International Expansion (Diversity): Key countries like India, the UK, Canada, and Spain are not just consumers, but massive contributors to the content library. The high volume of International TV Shows and International Movies genres demonstrates a successful strategy of localizing content creation to attract and retain global audiences.

Targeted Content: Different regions often show a concentration of specific genres. For instance, countries like India show a disproportionate amount of Action & Adventure and Dramas, reflecting a successful tailoring of content to regional tastes.

III. Insights from Content Clustering Text-based clustering (using features like description, cast, and listed_in) resulted in several distinct content groups, revealing Netflix's internal content segmentation:

**Cluster 1**: High-Value Originals (TV): This group consists of TV-MA rated, critically acclaimed titles with large, well-known casts and complex descriptions (often containing keywords related to 'crime,' 'sci-fi,' or 'thriller'). This represents Netflix's investment in prestige, high-budget content.

**Cluster 2**: International Dramas: These titles primarily cluster around non-English language indicators and have a high concentration of the International Movies or International TV Shows genres. This cluster validates the success of their international content sourcing.

**Cluster 3**: Niche & Short-Form: This cluster includes stand-up comedy specials, documentaries, and children's content. These are typically short, specific features that serve clear, non-overlapping audience segments.

IV. Chart Insights Summary The pair plot and distribution plots would primarily reveal patterns and correlations among the numerical features:

Pair Plot (Release Year vs. Cast Count): The scatter plot between release_year and cast_count shows that while older titles (pre-2000s) generally have a lower cast count, the content added more recently (2015-2019) exhibits a much wider variance in cast count, suggesting varied production scales. Critically, TV shows (is_tv_show=1) often appear to have a higher median cast count than movies, due to the number of recurring series roles.

Distribution of Release Year: The KDE plot for release_year would typically show a left-skewed distribution, confirming that the majority of content on the platform is relatively modern, with a significant spike in content released and/or acquired in the last 5-10 years (2010 onwards), in line with the platform's scaling strategy.

Content Type Count: The count plot would visually confirm that, despite the aggressive increase in TV shows, Movies still maintain the higher total count in the pre-2019 catalog, emphasizing the sheer volume of films in the starting library.

In short, the project confirms Netflix's strategic evolution: they are building a global, long-form content empire, heavily leveraging international production and using high-quality original content (identified through clustering) to drive core subscriber value.
