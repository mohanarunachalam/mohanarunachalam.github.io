---
title: What Can't Deep Learning Do?
published: true
layout: post
---

1/ What can't deep learning do? Worth putting together a list of known failures to guide algorithmic development.

2/ Deep learning methods are known to fail at learning after small jitters to input. Think object recognition breaking when colors are swapped.

3/ Gradient based learning is quite slow. Takes many, many gradient descent steps to pick up patterns. Tough for high dimensional prediction.

4/ Deep learning methods are terrible at handling constraints. Not possible to find solutions satisfying constraints unlike linear programming.

5/ Training for complex models is quite unstable. Neural turing machines and GANs often don't train well, with heavy dependence on rand seed.

6/ Unlike graphical models, deep networks aren't good at tying themselves to real world. Can't extract causal structures.

7/ For example, consider problem of influencer detection. Say senator voting dataset, want to detect key influencers. Not clear how with DNNs.

8/ Reinforcement learning methods are quite finicky. Performance depends critically on tuning tricks. This problem is endemic though.

9/ Deep learning can't reason about unknown entities easily. Consider video with baseball batter and pitcher offscreen.

10/ Not clear how to infer existence of pitcher in the world from DNN techniques.

11/ It's not really possible to train deep networks online (see above about slow training). So dynamic reactivity is hard.

12/ In general, behaviors will have to be learned offline for intelligent actions.

13/ People often bring up interpretability of deep nets. I think this isn't really as big a problem as people make it to be.

14/ But, it is hard to audit deep networks. How can we ensure that biased or racist things haven't been learned? See word2vec racism articles.

15/ DNNs can't easily solve logical problems. 3SAT solvers have powerful capabilities hard to put into deep nets.

16/ DNNs are terrible at handling wide feature scales. Unlike robust random forests, require heavy feature tuning.

17/ Hyperparameter search remains terrible. Practitioners either need heavy duty compute or lots of hand tweaking of architectures.

18/ This is by no means an exhaustive list. All of these are problems worth thinking about (and researching more).

19/ As an important question, are these problems intrinsic to deep networks, or are they engineering challenges to overcome?

20/ It's hard to say honestly. Some of these issues will likely be resolved. More hardware will likely allow for auto hyperparam search.

21/ There are some early architectural hacks to auto-normalize and handle large data scales, so feature handling might improve.

22/ However, the issues with logic, constraints, hidden structures, and auditing are likely deeper.

23/ I'd love to be proven wrong though. Deep learning practitioners are extraordinarily talented and imaginative.

24/ Plus, a version of Moore's law still holds for GPU performance (for how long though? can TPUs and custom hardware save us?)

25/ So, I'm relatively optimistic about these challenges. Nonetheless, I suspect deep networks are not sufficient for general intelligence.

26/ This might just be bad bias on my part though. Expert practitioners can be terrible at forecasting. Too much time in trenches.

27/ Leads to missing the forest for the trees.

28/ I've also resisted the urge to turn this tweetstorm into an essay. I don't yet know if there are underlying themes.

29/End Discovery and analysis left as an exercise to the discerning reader!

Acknowledgments: Adapted and expanded from a Twitter tweetstorm of mine. Thanks to twitter commenters who brought up some interesting additional points on the original thread (included here).
