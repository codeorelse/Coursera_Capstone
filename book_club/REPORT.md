# Finding a location for the first 'Book Club'

 ## Introduction
 
 We are working for a new (fictional) start-up called Book Club from Spain. [Data shows](https://publishingperspectives.com/2020/02/spain-new-reading-habits-report-digital-reading-up-29-percent/) that the Spanish stop reading books when they turn around 24, 25 years old, and they get back to reading in their mid-30's. And what is this group doing instead? Next to spending time with their family at home, they enjoy their spare time in the city to go out and have fun. The main reason for reading less, they say, is the lack of time. 
 
 So The Book Club wants to offer the Spanish a place where can have the feeling of going out with friends, away from home and obligations, but still do something they deep down really love: reading. The Book Club is a club where there are silent rooms where you can read books, but it also has a hall for experimental music and literature events. Your  can bring your own book to The Book Club, or one can rent a book, both physical as digital, at the venue. All books that can be rented at The Book Club are supplied by local book stores, so by coming to The Book Club you also support local businesses.

 ## Business Problem

Book Club wants to start their first club in [one of top party cities in Spain](https://gogoespana.com/en/blog/spains-top-party-cities/): Barcelona. But now they've picked the city the next big question: __in what district should we start looking for a property for the first Book Club__? There a few criteria:

1. As the target audience for The Book Club are _barcelonians_ between 24 and 35 year, we are looking for districts where these people are living. 
2. The Book Club really wants to focus on bringing the _barcelonians_ in, and not a lot of tourists. Therefore, The Books Club can not be located near a lot of popular tourists attractions. 
3. As it's still a club, and it would be nice if people can go from the Book Club to let's say a dance club when they are done reading, or vica versa, we would like the Book Club to be located in a district with at least two other clubs. 
4. The Book Club is a non-profit organisation, and there is not a lot of money to spend on the rent, yet, so we should also take the average rent of the district into account.

 ## Data sources

### Population data

For information about the Barcelona population, I will use the available data sets from [Barcelona Open Data BCN](https://opendata-ajuntament.barcelona.cat/en). I will primaraly use the [Official population figures. Population of the city of Barcelona according to age and sex](https://opendata-ajuntament.barcelona.cat/data/en/dataset/est-ine-edat-any-a-any/resource/2c0600f5-4c78-4b14-b4c1-873244425865) data set to get information about the age groups per district. 

### Existing clubs and tourist attractions

We will use the Foursquare API to find existing clubs in Barcelona. Also, we will find all the location information about touristic attractions in the city using Foursquare. I will query the Foursquare API for the most popular tourist attraction names that I will find using web pages like https://ticketshop.barcelona which list popular tourist spots in Barcelona. 

### Club meta data

Because we are mostly interested in neighbourhoods where locals between 24-35 go clubbing, we will also need to do some deep dives in the clubs in the city. Not only their location, but also their audience is interesting to solve the business problem. There is no public data set available with this data, so we will need to do some extra research on the clubs to find their audience. I will do this by Googling the club names, find photos, find reviews, see what people say about these clubs. 

### Tourism data

Alhthough I haven't found a kwantative data set about tourism in Barcelona, the city published a [Tourism activity report](https://ajuntament.barcelona.cat/turisme/sites/default/files/iat19_1.pdf) every year that holds a lot of information that will come in handy with the business problem. 

### Real estate pricing

To get an idea of the average price for real estate in Barcelona per district, I will use the [Price of purchase of registered properties of the city of Barcelona](https://opendata-ajuntament.barcelona.cat/data/en/dataset/est-mercat-immobiliari-compravenda-preu-total) and [Average monthly rent (€ / month) and average rent per surface (€ / m2 per month) of the city of Barcelona](https://opendata-ajuntament.barcelona.cat/data/en/dataset/est-mercat-immobiliari-lloguer-mitja-mensual).

### Spanish reading habits

To find more insights on the Spanish reading habits, I will look at some extra reports like 
[Barometer of Reading Habits](https://publishingperspectives.com/2020/02/spain-new-reading-habits-report-digital-reading-up-29-percent/). These might give me extra informations and new directions during the data analysis and business problem solving. 