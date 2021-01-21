# Deep-Q-Learning-tensorflow
Here we use a deep q learning network to simulate traffic control, over a UI build on Tkinter

# Car select fastest route to the destination
 -environment: streets of a city
 -state: traffic that there is at any given point of time
 -Agent: A car
 -Action: Turns (navigate the environment and make decisions (turns))

Now in this case we have many cars that are going to be taking decisions based on the decision of the other agents as well. So here is where it can get complicated.

The goal for one car is clear, to arrive faster to the destination. But, should we keep this goal when we have many agents making decisions in the same environment?

If we keep the same goal, each car will still be trying to find the way by its own, but it may take the route that limits the other cars and they will increase their own travel time.

Instead, we should make the goal to reduce the average travel time of the cars, so the optimization works for every car in the environment.

Now each car will make decisions based not only in themselves but also regarding other cars, in order to avoid a much bigger traffic jam.

The multi-agent case also raises the concern of  how much time does a car can sacrifice to avoid disturbing others cars travel time.

Ref : https://medium.com/yellowme/deep-reinforcement-learning-dqn-for-multi-agent-environment-5f4fae1a9ff5
