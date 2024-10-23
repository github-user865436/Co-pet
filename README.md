# Co-pet
My TrackMania AI.

# Network layers
Inputs:

The inputs given will start at ray cast distances and what is hit. The rays only hit solid objects and triggers and although water will be considered a surface type, we will only consider solid surfaces when stopping the rays. Two other inputs will be the angle the car is moving towards on both X and Y planes. All the currently said inputs are relative to the vehicle and camera angle. The speeds will be measured in rotation and base. A negative for the rotation speed number means counterclockwise rotation and vice versa. On the other hand, a negative for base speed would mean you are going backward that fast instead of going forward. The last things I will give my neural network are the car’s pitch and roll, the game engine and if it uses deterministic physics, the car type, and car boosts like car retraction.

Outputs:

All I want from outputs is to press accelerate or break, and a steer value with negative being left and positive being right.

Hidden:

Explain here what our AI pieces together to result in what it does.



# About rewards
Short-term:

If we have less reward at a certain point of the race, it means we could improve there and that the provided outputs could still be altered to change the outcome of the race to be better and in our favor. However, having more rewards means the opposite; we could only make minimal changes to improve. We can compute short-term rewards by being given a certain time and performance in a race. The reward will be low if our Artificial Intelligence has not completed many small goals. Please note that, although not mentioned, short-term rewards also give more on parts done well even if other parts are worse since those parts are punished on a long-term and not short-term basis. The rewards are given short-term and our AI itself has similar growth patterns when it comes to calculating the rewards it is being given in the first place. This will make the rewards being given, calculated exponentially but because of progress barriers, it makes it look like there is no exponential growth but instead makes it look like short progress gaps are still good later into training systems.

Long-term:

Failing races results in terrible long-term rewards because based on the race length, you will receive more or less—worse—punishments. If the race is short, we will receive less punishment for failing. Vice versa applies to when the race is long. If the race is complete: taking longer results in less reward than you would for completing in optimal times. Similar to what is currently written, long-term rewards focus more on how we should be rewarded or punished for how we have performed in the race. Long-term rewards do not grade based on how optimally you played at certain parts but instead, if you finished optimally. Finishing times are graded through rewards and punishments because our AI will attempt to get as many rewards as possible short-term instead of also noticing finishing time. If our AI is heavily influenced by finishing times, it will want to do more risky things to help itself a little later on in the race.

Analogies for how cars will obtain rewards:

Say at a certain time in a race, there are thousands of cars in a similar section. If you overlapped these, it would be absolute chaos. But if you also took the front cars versus the back ones, you’d find the front cars getting the higher short-term reward. But what if all the cars kept good pace with each other in comparison to race length, and the front cars fell off with the end not far, in sight? This would give the previous back cars good long-term rewards. But what if the back cars get a lead instead of the front cars falling off? Then the now, the front cars will still get a better long-term reward than the now-back cars.

How the types of rewards will be used:

It has already been mentioned that Artificial Intelligence has given information on improvement. But in actuality, our AI is told how and where to potentially improve but is never told what to improve because it must figure this out on its own by natural selection and randomness. This section is dedicated to how our AI will use these rewards to mix in what I just mentioned and therefore, improve.



# How the AI will evolve
Example
Example



# Machine-learning algorithms
Example
Example



# Notes 
Explore new techniques created randomly by our AI.


