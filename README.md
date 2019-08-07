# Leveraging Twitter to Map Disasters
--------
#### Problem Statement:
###### Data Science Perspective:
- Is it possible to develop a tool that, using a set of keywords, can identify natural disasters events and, from that information, discern the geolocation of said disaster?
###### Client Perspective:
- The client has asked us to provide a tool that, through the usage of a customizable list of keywords that corresponds to disasters, monitors live streams of social media posts (in this case, Twitter) and then provides the geolocation of each post.

#### Executive Summary
- Ultimately, we were able to create a tool that allows the client to input a customizable list of words that returns the geolocations of tweets that correspond with certain disasters. Our tool should be considered a prototype at best because of the sizable amount of noise that gets labelled improperly alongside true disasters. In our case, training a machine learning model to generalize to multiple different types of disaster did not work well. For best results, models should be trained on datasets that pertain to specific natural disasters (e.g fire data when looking for fire tweets, flood data when looking for flood tweets).

#### Background Info
- Because of external factors like Climate Change, certain natural disasters like wildfires and hurricanes/typhoons are increasing over time. Due in most part to modern technology, the amount of deaths per natural disaster has gone down over time, despite the increasing frequency of such disasters. The goal of a project like this is to aid in further decreasing the number of deaths that occur when a natural disaster hits. Ideally, by getting the geo-locations of tweets that pertain to disasters, emergency response teams can quickly ascertain where a disaster hit and where to focus their resources.


#### Analysis
 - We created a tool for our client that can take a customized list of keywords and return the tweets that correspond to those keywords. It can then identify which of those tweets likely indicate disaster and it can also give the geolocation of each tweet, but, as stated before, it does have limitations.
 - ***Limitations***: Because of large amounts of noise in our dataset, as well as the inability of our tool to work for multiple disasters at a time, there is still a lot of work that needs to be done in the future for this tool to be considered complete and implementable in the case of an actual disaster striking.
 #### Future Recommendations
 - ***Data Gathering and Hand Labelling***: If we had more hand labelled tweets pertaining to specific disasters, the model could be better trained to hone in on more specific keywords that are used when disaster strikes. 
 - ***Removing and Adding Weight Words***: If certain words like "Sandy", "Katrina", and other very specific singular disaster words were to be added to stopwords, the model would likely generalize better to disasters. This has yet to be tested though. If there ere also ways to add in certain words as weight words that the model may not have caught when training itself, that could also help.
#### Outside Sources
- All data used in this project came from two sources. Training datasets all came from crisislex.org and all testing data came from using Twitter’s API.
