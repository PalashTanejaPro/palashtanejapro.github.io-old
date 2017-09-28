---
published: false
---
##Introduction
Markov chains, named after Andrey Markov, are mathematical systems that hop from one "state" (a situation or set of values) to another. For example, if you made a Markov chain model of a baby's behavior, you might include "playing," "eating", "sleeping," and "crying" as states, which together with other behaviors could form a 'state space': a list of all possible states. In addition, on top of the state space, a Markov chain tells you the probabilitiy of hopping, or "transitioning," from one state to any other state---e.g., the chance that a baby currently playing will fall asleep in the next five minutes without crying first.

Even though they are overshadowed by Deep Learning Models like RNNs and DNNs, they prove to be very effective in sentence generation tasks. We have all seen the autocorrect predictions on our phones, in fact they are based on Markov chains and they can be tapped repeatedly to generate loopy sentences.

I wanted to do something interesting and comedic with Markov Chains so I decided to make a Donald Trump tweet bot from a Trump tweet dataset. 