---
title: Making Realistic Twitter Bots Using Markov Chains
published: true
---

### Introduction

Markov chains, named after Andrey Markov, are mathematical systems that hop from one "state" (a situation or set of values) to another. For example, if you made a Markov chain model of a baby's behavior, you might include "playing," "eating", "sleeping," and "crying" as states, which together with other behaviors could form a 'state space': a list of all possible states. In addition, on top of the state space, a Markov chain tells you the probabilitiy of hopping, or "transitioning," from one state to any other state---e.g., the chance that a baby currently playing will fall asleep in the next five minutes without crying first.

Even though they are overshadowed by Deep Learning Models like RNNs and DNNs, they prove to be very effective in sentence generation tasks. We have all seen the autocorrect predictions on our phones, in fact they are based on Markov chains and they can be tapped repeatedly to generate loopy sentences.

[Here is a great introduction to markov chains.](http://setosa.io/ev/markov-chains/)
### Implementation

I wanted to do something interesting and comedic with Markov Chains so I decided to make a Donald Trump tweet bot from a [Trump tweet dataset.](https://www.kaggle.com/kingburrito666/better-donald-trump-tweets) and made a state 2 Markov Chain from it.
I used the tweepy library for Python to create the Twitter Bot.
~~~python
import tweepy, time, sys
import markovify

 
#enter the corresponding information from your Twitter application:
CONSUMER_KEY = 'KEY' #keep the quotes, replace this with your consumer key
CONSUMER_SECRET = 'SECRET' #keep the quotes, replace this with your consumer secret key
ACCESS_KEY = 'KEY' #keep the quotes, replace this with your access token
ACCESS_SECRET = 'SECRET' #keep the quotes, replace this with your access token secret
auth = tweepy.OAuthHandler(CONSUMER_KEY, CONSUMER_SECRET)
auth.set_access_token(ACCESS_KEY, ACCESS_SECRET)
api = tweepy.API(auth)
 
model_json = open('sav1.json').read()
model = markovify.Text.from_json(model_json)

line = model.make_short_sentence(200)

api.update_status(line)
print("Tweet Made: ",line)
time.sleep(900) #Tweet every 15 minutes
~~~

### Results

My bot [McDonaldTrump](https://twitter.com/__McDonaldTrump) is puts out about 50-60% grammatically incorrect and incoherent tweets but the remaining ones are *worth a laugh!*

**Here are a few that I liked:**


* <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Get rid of the others?An incredible honor to be <a href="https://twitter.com/hashtag/AmericaFirst?src=hash&amp;ref_src=twsrc%5Etfw">#AmericaFirst</a>!</p>&mdash; Donald Trump (@__McDonaldTrump) <a href="https://twitter.com/__McDonaldTrump/status/912944443879239680?ref_src=twsrc%5Etfw">September 27, 2017</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script><br>


* <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">People are not true- just like we have no country.</p>&mdash; Donald Trump (@__McDonaldTrump) <a href="https://twitter.com/__McDonaldTrump/status/912232902351519744?ref_src=twsrc%5Etfw">September 25, 2017</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script><br>



* <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Go out and build a WALL!.<a href="https://twitter.com/KatrinaCampins?ref_src=twsrc%5Etfw">@KatrinaCampins</a> Thank you to the end result was solid!Dishonest media is able to extort $1,000,000.00 from me.</p>&mdash; Donald Trump (@__McDonaldTrump) <a href="https://twitter.com/__McDonaldTrump/status/912251927349559296?ref_src=twsrc%5Etfw">September 25, 2017</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script><br>