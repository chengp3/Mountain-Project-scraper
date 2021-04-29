# Rock climbing

Every cliff that is frequently climbed is well characterized with different properties. This varies from gear type (bouldering, sport, trad, aid, ice...) to difficulty (on the "Yosemite scale"- 5.0 to 5.16), its geolocation, etc. This data is stored in the community's collective memory, in guidebooks, and online on different websites, the most popular being the <i>Mountain Project</i>, the wiki of outdoor rock climbing. MP is generally used as a reference, but you can also make an account there and "tick" climbs off, which show up on your profile like a trophy wall of sorts. 

This is the scraper made to pull information from Mountain Project. MP used to have an API until recently when it was bought by a private company that promptly shut off the API with no plans to monetize. ...

This scraper downloads the entire website and puts it into a database, with the end goal of feeding it into another project of mine ("the proj proj" repo) that generates useful/pretty graphs to help climbers visualize their evolution as climbers. 

1. Database.ipynb -- the initial scrape, starts with a tree structure of MP site urls and ends with a database of routes with corresponding details
2. Tick DB.ipynb -- tools to scrape a person's tick list, and join the list with the route database to pull up data on all of a person's ticks
3. Max Grade Chart.ipynb -- analyze how hard a person climbs over time
4. Style Analysis Chart.ipynb -- tools to scrape each route description to classify the route character (slab, face, overhang, crack, etc)
5. Final.ipynb -- some projproj specific utilities to make the site run more smoothly

Check out the alpha site at pcheng3.pythonanywhere.com
