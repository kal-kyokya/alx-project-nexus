# Movie recommendation System/Algorithm

## Futtech:
	- Video Recommendation System/Algorithm
---

### Friday, 8th August 2025, 11:25 AM

* What is the end goal of this 'feature'?
--> Generate a set of videos a user X will most likely be pleased to watch.

* Interesting. Where are the videos coming from?
--> There is a pool of videos from which we will extract the set.
    I'm talking about all the uploaded content to Futtech.

* 'all the uploaded content to Futtech' sounds a bit vague to me, care to clarify?
--> Yes, sure.
    At the end of the day, every single bit of information associated with Futtech
is to be stored in the project's database.
    'Everything will be stored or referenced inside the DB.'
    As far as videos are concerned, data will be spread across 3 services;
	* A CDN (Same thing as Object Storage?)
	* A cache (Redis, reduce DB hits)
	* The Database
    So yeah, the set of recommended videos will be extracted from this trio of 
data storing structures.

* Thanks for that. What mental model best represents this recommendation system?
--> At this point in the conversation, the 'black box' model looks completed.
	'INPUT ==> BLACK BOX ==> OUTPUT'
    We have defined where the data comes from and what data is expected, just gotta
complete the model by discussing how exactly the input is used to generate the output.
---
