# Movie recommendation System/Algorithm

## Futtech:
	Video Recommendation System/Algorithm

---

### Friday, 8th August 2025, 11:25 AM

* What is the end goal of this 'feature'?
<br />--> Generate a set of videos a user X will most likely be pleased to watch.

* Interesting. Where are the videos coming from?
<br />--> There is a pool of videos from which we will extract the set.
<br />    I'm talking about all the uploaded content to Futtech.

* 'all the uploaded content to Futtech' sounds a bit vague to me, care to clarify?
<br />--> Yes, sure.
<br />    At the end of the day, every single bit of information associated with Futtech is to be stored in the project's database.
<br />    'Everything will be stored or referenced inside the DB.'
<br />    As far as videos are concerned, data will be spread across 3 services;
	* A CDN (Same thing as Object Storage?)
	* A cache (Redis, reduce DB hits)
	* The Database
<br />So yeah, the set of recommended videos will be extracted from this trio of data storing structures.

* Thanks for that. What mental model best represents this recommendation system?
<br />--> At this point in the conversation, the 'black box' model looks completed.
<br />	'INPUT ==> BLACK BOX ==> OUTPUT'
<br />    We have defined where the data comes from and what data is expected, just gotta complete the model by discussing how exactly the input is used to generate the output.

---

### Saturday, 9th August 2025, 11:48 AM

* The 'black box' model, interesting. What's your guess on its operating principles?
<br />--> I believe usage of DB fields; Rating, Likes, Views, Created at will facilitate creation of a filtering criteria that will extract a different set of X items from the Video model each time.
<br />    I'm thinking of a set comprising of:
	* The highest-rated videos.
	* The most liked ones.
	* Those with the greatest number of views.
	* The most recently uploaded ones.
	* Those with views/created_at ratios above a certain treshold (Rising stars)
<br />2 of each should yield 10 videos to be recommended to the user by this system.
<br />    This works best for large datasets though. Hard to get a varied answer with a DB that has, say 20 videos and similar ratings and/or likes.

* Huuum, that's a detailed answer right there. Anything else you'd like to say?
<br />--> Without putting too much thought into it, I think of two types of recommendation systems; video-based & user-centered.
<br />    The set of recommended videos can be dependent on the attributes associated with the Video model or the User model. What I described previously is a video-based. The alternative would be a set of videos selected off of the types of videos a particular user liked, rated, viewed or created.
<br />    In something of a philosophical sense, one is about providing the user with 'the best the world has to offer', while the other is about 'that which matches your personality and character'.
<br />    Objective and Subjective realities, innit?
<br />
<br />    In the initial stages of development, I will stick to the 'Objective' approach, a single set of recommended videos for every user that is computed daily.
<br />    Once the Futtech has enough videos and/or users, I will consider satisfying each user with targeted and well curated sets.

---
