---
layout: post
title:  RL Squared
---

<center>
    <iframe width="720" height="400"
    src="https://www.youtube.com/embed/ZWH6Dsueeps">
    </iframe>
</center>

Looking back, I think the name of the project was a lot lamer than the three of us thought it was. We thought we were so clever combining the RL from Rocket League + the RL from Reinforcement Learning. This project was one of the few that I was most proud of. Strangely enough, the spring quarter of my junior year had a ton of really difficult, but interesting courses to take (Computer Security, Reinforcement Learning, Distributed Systems, and AR/VR). Of these classes, I'd say that the RL class and AR/VR class had the best final projects. 

We started off the project super ambitious and thought that we would be able to create a 2v2 bot that would be able to beat us in Rocket League. To be fair, of the three of us working on the project, only one of us knew how to play. However, we would start to run into a whole bunch of issues that would cause use to slash the scope of the project as the deadline came closer.

Firstly, getting replay data from Rocket League is super annoying as the game doesn't actually record the inputs of all players during replays, only their positions. This would mean that our model wouldn't be able to know what moves the players were doing in order to learn from them.

So, we decided to work with model distillation, basically training a smaller model off the outputs of a larger model. We chose to use Nexto, the current best Rocket League model, as our larger model. However, this was too effective and the model was essentially a worse version of Nexto and any training that we did had little to no effect on the model as it was basically too good for us to work with.

So, we decided to experiment with different modern reinforcement learning techniques in order to see how they performed at a simple task in Rocket League, dribbling the ball. In this game, that's essentially balancing the ball on the top of the car. We felt that this was a good enough test as it mirrored the inverted pendulum problem (a common RL benchmark), but more complex.

One of my teammates also insisted that we did all reports in LaTeX, which was super annoying at first. But come on man, look at how cool our report looks.

<embed src="{{ site.baseurl }}/assets/RL_2_Final_Report.pdf" width="720" height="1000" type="application/pdf">

