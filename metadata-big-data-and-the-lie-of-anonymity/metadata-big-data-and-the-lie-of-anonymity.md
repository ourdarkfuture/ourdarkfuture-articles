![](phone.jpg)

Whenever some company or government organization unveils some massive, privacy invading technology, the reveal is always immediately accompanied with qualifications that "don't worry, the data is anonymized." PR departments assure us that trustworthy computer code scrubs everything that could identify us individually from the vat of indistinguishable data.

Of course that's just a convenient lie.

Researchers from Stanford published a paper today entitled "[Evaluating the privacy properties of telephone metadata](http://www.pnas.org/content/113/20/5536.full)" in the *Proceedings of the National Academy of Sciences*. The research attempts to quantify just how much individual information can be gathered from "anonymous" metadata.

It turns out it's a lot.

The study used 800 volunteers who ran a special smartphone application that recorded basic call and text metadata (numbers communicated with as well as how often and for how long). A quarter of a million calls and over a million text messages were collected and then analyzed, mostly with simple and cheap automatic tools.

The results of the study were broken down into a few main areas: re-identification, location inference, relationship inference, sensitive trait inference, and scope. In short, they discovered it was trivial to identify who you are, where you are, if you're in a relationship, and sensitive personal information. Further they found that the "restrictions" on the NSA's metadata collection program likely meant nearly every American was able to be surveilled and millions (potentially tens and hundreds) may continue to qualify. But let's take a closer look.

####Scope

The [Oracle of Bacon](http://oracleofbacon.org/) is a fun take on the [six degrees of separation trope](https://en.wikipedia.org/wiki/Six_degrees_of_separation) which suggests that everyone in the world is only six "hops" away from anyone else. In the game, you try and find the least amount of connections between actors (or anyone in film) and Kevin Bacon based on what movies they've worked on. For example, you follow actor A who worked with actor B on film X, then actor B who worked with Mr. Bacon on film Y (my Bacon number is 2 for those keeping track).

Well it turns out that the NSA's restriction on metadata collection is essentially a national security version of the Oracle of Bacon. Since 2013, the NSA is restricted to only "two-hops" (and before it was virtually unlimited) which, according to the findings of the researches) means a single suspect can lead to approximately 25,000 "second hop" individuals who qualify for surveillance. To put it another way *less than 10,000 suspects could allow every adult in the United States to be surveilled.* For those keeping track, the current watch list is in the [tens of thousands](http://www.factcheck.org/2015/12/rubio-on-terrorist-watchlist/).

###Re-identification

The saving grace for these programs has always been the claim that "it's just anonymous metadata, it can't be used to identify individuals." Researchers put that to the test using simple and cheap datasets and techniques. Using only an automatic search on publicly available databases (Google, Facebook, and Yelp) they were able to immediately identify 32% (9,576) of the numbers collected.

The study then set aside 250 randomly selected numbers to test if more advanced identification was possible. For just $19.95 a month, the researchers subscribed to the [Intelius](http://www.intelius.com/) database and proceeded to manually search the selected numbers there and on Google. In just 70 minutes of web searching, Intelius had matched 65% of the numbers with Google matching 58% for a total of 82% of metadata matched to individuals. They did this within the limitations of this publicly available data and almost no monetary resources, suggesting that government or well funded organizations could easily get close to 100% re-identification.

####Location

Just like the PR declarations of "anonymous" metadata, we've heard over and over how location data is not collected. Well it turns out that location is trivial to identify as well. Using information on what businesses subjects called and data from Facebook, 60% of the 250 individuals selected for advanced analysis were correctly identified as living in a specific city (within 5 miles) and nearly 90% were identified correctly within 45 miles.

####Relationships

The researchers took all this a step further to identify if an individual was in a relationship and if so with who. They trained a [support vector machine](https://en.wikipedia.org/wiki/Support_vector_machine) (a learning algorithm that places data in one of two categories) that had great success in correctly identifying individuals in relationships automatically. Once a relationship was identified, it was simple for them to identify who that relationship was with based on the number of calls (81% accuracy), number of days calling (77% accuracy), number of texts (76% accuracy) and days with a text (76% accuracy). Additional metrics like text and call length provided additional points for confirmation.

####Sensitive Traits

Most alarming and damning for the "anonymity" of metadata, was the ability of researchers to discern "private" information based solely on who individuals are communicating with. This info included confidential health information and potential knowledge of illegal activities. See their examples below:

>i) Participant A held conversations with a pharmacy specializing in chronic care, a patient service that coordinates management for serious conditions, several local neurology practices, and a pharmaceutical hotline for a prescription drug used solely to manage the symptoms and progression of relapsing-remitting multiple sclerosis.

>ii) Participant B received a long phone call from the cardiology group at a regional medical center, talked briefly with a medical laboratory, answered several short calls from a local drugstore, and made brief calls to a self-reporting hotline for a cardiac arrhythmia monitoring device.

>iii) Participant C placed frequent calls to a local firearm dealer that prominently advertises a specialty in the AR semiautomatic rifle platform. He also placed lengthy calls to the customer support hotline for a major firearm manufacturer; the manufacturer produces a popular AR line of rifles.

>iv) Participant D placed calls to a hardware outlet, locksmiths, a hydroponics store, and a head shop in under 3 weeks.

>v) Participant E made a lengthy phone call to her sister early one morning. Then, 2 days later, she called a nearby Planned Parenthood clinic several times. Two weeks later, she placed brief additional calls to Planned Parenthood, and she placed another short call 1 month after.

Several of these vignettes were confirmed with public sources. Beyond that, even if what is implied by some of this data is not true, the mere fact that it is suggested could post trouble for an individual and is obviously a deep invasion of privacy.

###Time to Confront This

If you're an advertiser or government organization hiding your tracking behind claims of "anonymized" data, you need to stop. Admit that you are tracking individuals and can trivially identify them if the need or want arises. Justify your tracking through the benefits you believe it offers (good luck with that) instead of hiding behind the PR shields of "anonymity."

Metadata, with enough data and time, exposes the details of our lives to anyone who makes the effort to connect the dots. As automated processing and machine learning grow in leaps and bounds, these dots are being increasingly connected and are ripe for commercial, criminal, and/or governmental abuse and exploitation. It's important that our dialogs on anonymous data be motivated by this and other scientific researchof the true extent of this "anonymity" instead of the conventional wisdom and gut feelings of law makers who aren't aware of what current technology is capable of.

***

Thanks to Stanford, Jonathan Mayera, Patrick Mutchlera, and John C. Mitchell for putting the time, money, and effort into this research.



