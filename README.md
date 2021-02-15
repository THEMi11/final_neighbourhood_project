# final_neighbourhood_project
Exploring Moscow neighbourhoods

Introduction
This project could be helpful for the people who is searching for similar neighbourhoods or for neighbourhoods 
most suitable for living there or to spent time in there. So, they could compare their own neighbourhood with 
others in case of moving, or they could clear up where are the best places for entertainment.

Data
I took the data form wikipedia districts page. I cleared the data and then added location data to the dataframe
by using geocoder library. With coordinates I formed a request to foursquare api and received venues data for 
all districts. Then, I used the elbow method to discover optimal k-value for Kmeans model. I fit the model 
after and found out that there are two major clusters. After seeing their features i assumed that there are 
(leisure/eentertainment) districts, and living area districts (places specifially designed for living there). 
So in the first category there was a lot of restaurants, boutiques, pubs, shops. but in second one there was 
many supermarkets, pharmacies, parks, sport complexes, coffee shops etc.

Components
Data was imported with BeautifulSoup library. Then added to dataframe and cleared with pandas. The location data 
was provided by geocoder library. With folium framework was created map of the Moscow city, and all the 
neighbourhoods was placed on it. Then I formed forsquare API request to receive the data about venues in each 
neighbourhood. One hot encoding was used to create dataframe suitable fo Kmeans method. Using the Elbow Method 
I found optimal k-value for Kmeans. Then i applied Kmeans clusterisation method on final dataset.

Results/Conclusion
Finally, I found out that there are two major clusters. After seeing their features i assumed that there are 
(leisure/eentertainment) districts, and living area districts (places specifially designed for living there). 
So in the first category there was a lot of restaurants, boutiques, pubs, shops. but in second one there was 
many supermarkets, pharmacies, parks, sport complexes, coffee shops etc.
