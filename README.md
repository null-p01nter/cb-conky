#About
This is a simple Conky .conkyrc configuration file.  It writes some information about the system as well as the local weather and a BBC news feed.

![Alt text](/screenshot.png "The script, running on CrunchBang Linux")

#Editing Weather
Currently, the weather is configured to State College, PA.  To change it to your locale, you must first find the Yahoo weather ID.  Visit http://weather.yahoo.com/ and search for your city or zip code. You'll be brought to a page like http://weather.yahoo.com/united-states/pennsylvania/college-28745304/.  The number at the end (in this case, 2499253) is your weather ID. Edit .conkyrc on line 91 and change http://weather.yahooapis.com/forecastrss?w=2499253&u=f to have your proper weather ID. 

#Editing News
The default needs feed is BBC News - Home.  This can be easily adjusted by replacing lines like 1. ${rss http://feeds.bbci.co.uk/news/rss.xml 4 item_title 1} to the rss feed of your choosing.
