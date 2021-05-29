# Code Summary
This code takes a country shapefile and any document and scans it for city names. When it collects those city names, it outputs two maps and a graph. The first map is a representation of all the cities where darker colors over areas for cities that are mentioned more. The second map shows all the cities using Folium to edit the apperance of the map. The chart was a graph of the frequency of each other cities mentioned. 

# Debugging 
I didn't need to do any debugging! 

# Reflection 
Is the gazetteer we're using appropriate for the text? What might be some of the challenges of using Nominatim with a book published in 1859?
The gazetteer we're using was appropriate for Mark Twaine's novel, because the novel includes a lot of very clear, different cities and places. It isn't as appropriate for a project like my geography paper, because I use a lot of informal place names and because I'm talking about how the city has changed over time, I am talking about places that have changed names over time. Nominatin might struggle with a book published in 1859 for that very reason. Places might have changed names, shifted location, or even altered simple spellings or geographic boundaries over time. 

How accurate do you think the outputs are? Are there any city names that seem suspect? If so, what are some Natural Language Processing methods that you could use to filter words that might be city names, but probably weren't intended as city references in the text?
I don't think the output was very accurate at all. Many of the building or street names in San Francisco were mapped to cities outside the San Francisco or even outside the United States. By including a language processing method that recognized the term "street" or checked if "street / road / blvd / etc" after each city name. That would help filter out false finds, or misindentified cities that are actually streets. 

What are some alternative approaches to mapping the data? The tutorial here uses duplicate entries and opacity to present a type of "color ramp": could this be done better?
I think that it could have been done better if you altered the size of the trianges but on the frequency of the mention. I think that would have really shown which places are commonly mentioned and which are less commonly mentioned. Alternatively, without using duplicate entries, you could just show a map of all the cities, such as the map produced by Folium. I did think the opacity is very effective as well. 
