#  **Data Sourcing Challenge**
### By: Kyle Kerner

In this program we access the New York Times and The Movie Database APIs.  Starting witht the New York Times API we filter by section names of: Moives, types of materialsL Review, and headline: Love, sorted by newest, returning headline, web_url, snippet, source, keywords, pub date, byline, and word count, through 20130101 to 20230531.  From there we retieve 200 results from the first 20 pages by looping through the API, montioring the API limits and add the results to reviews_list. Reviewing the data it is normalized can converted to a Pandas DataFrame.  The title of the DataFrame is extracted and added to a titles list.  

Once the titles list is created and populated The Movie Database API is search to see if there is a title matching titles within the API.  The matching results are added to tmdb_movies_list while monitoring the API limits. Matching results pull specified data points that are added to tmdb_movies_list and converted to a DataFrame

Once the DataFrame is completed for the Movie Database API the two created DataFrames for each API are merged on title and columns/characters are manipulated to create a cleaner DataFrame.  Once cleaned the DataFrame is exported to a CSV file. 

# Sources
Source code provided in class as well as the use of Chat GPT to help with code direction was used in the making of the program.  