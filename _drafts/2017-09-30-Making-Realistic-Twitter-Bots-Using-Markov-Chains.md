---
published: false
---
##Introduction
Markov chains, named after Andrey Markov, are mathematical systems that hop from one "state" (a situation or set of values) to another. For example, if you made a Markov chain model of a baby's behavior, you might include "playing," "eating", "sleeping," and "crying" as states, which together with other behaviors could form a 'state space': a list of all possible states. In addition, on top of the state space, a Markov chain tells you the probabilitiy of hopping, or "transitioning," from one state to any other state---e.g., the chance that a baby currently playing will fall asleep in the next five minutes without crying first.

Even though they are overshadowed by Deep Learning Models like RNNs and DNNs, they prove to be very effective in sentence generation tasks. We have all seen the autocorrect predictions on our phones, in fact they are based on Markov chains and they can be tapped repeatedly to generate loopy sentences.

##Implementation
I wanted to do something interesting and comedic with Markov Chains so I decided to make a Donald Trump tweet bot from a [Trump tweet dataset.](https://www.kaggle.com/kingburrito666/better-donald-trump-tweets) and trained a state 2 Markov Chain on it.
Then I used the tweepy library for Python and set my model loose on Twitter! It has not failed to surprise me in the 2 days that it has been alive.

##Results
My bot [McDonaldTrump](https://twitter.com/__McDonaldTrump) is puts out about 50-60% grammatically incorrect and incoherent tweets but the remaining ones are *worth a laugh!*

**Here are a few that I especially enjoyed:**
<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">MAKE AMERICA GREAT AGAIN!Join my team of deplorables for tonights <a href="https://twitter.com/hashtag/debate?src=hash&amp;ref_src=twsrc%5Etfw">#debate</a> <a href="https://twitter.com/hashtag/MakeAmericaGreatAgainUNBELIEVABLE?src=hash&amp;ref_src=twsrc%5Etfw">#MakeAmericaGreatAgainUNBELIEVABLE</a>!</p>&mdash; Donald Trump (@__McDonaldTrump) <a href="https://twitter.com/__McDonaldTrump/status/913465988393422849?ref_src=twsrc%5Etfw">September 28, 2017</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Get rid of the others?An incredible honor to be <a href="https://twitter.com/hashtag/AmericaFirst?src=hash&amp;ref_src=twsrc%5Etfw">#AmericaFirst</a>!</p>&mdash; Donald Trump (@__McDonaldTrump) <a href="https://twitter.com/__McDonaldTrump/status/912944443879239680?ref_src=twsrc%5Etfw">September 27, 2017</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
*Sometimes he gets really spiritual*
<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">People are not true- just like we have no country.</p>&mdash; Donald Trump (@__McDonaldTrump) <a href="https://twitter.com/__McDonaldTrump/status/912232902351519744?ref_src=twsrc%5Etfw">September 25, 2017</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
*And I will leave you with that one*
<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Go out and build a WALL!.<a href="https://twitter.com/KatrinaCampins?ref_src=twsrc%5Etfw">@KatrinaCampins</a> Thank you to the end result was solid!Dishonest media is able to extort $1,000,000.00 from me.</p>&mdash; Donald Trump (@__McDonaldTrump) <a href="https://twitter.com/__McDonaldTrump/status/912251927349559296?ref_src=twsrc%5Etfw">September 25, 2017</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>