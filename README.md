# Co-pet
My TrackMania AI.

Network layers
Inputs
Ray cast distances and what is hit relative to car and camera angle and can only hit solid objects and triggers and although water will be considered as a surface type, we will only consider solid surfaces when stopping the rays
Angle car is moving towards X relative to car and camera angle
Angle car is moving towards Y relative to car and camera angle
rotation speed 
    negative = counterclockwise
    positive = clockwise
Car speed
    negative = backwards
    positive = forwards 
Pitch
Roll
Deterministic game
Game engine
Car type
Car boosts

Outputs 
Accelerate
Break
Steer
    negative = left
    positive = right

Middle
Reformat explanations for the layers in standard text like so and explain here what the AI pieces together to result in what it does.

About rewards
Short-term:
If we have less reward at a certain point of the race, it means we could improve there and that the provided outputs could be altered to change the outcome of the race in our favor. 
However, having more reward means the opposite and therefore, we could only make minimal change to improve. We can compute short-term rewards by being given a certain time and performance on a race. If our AI has not completed many small goals, the reward will be low. Please do note that, although not mentioned, short-term rewards do also give more on parts done well on even if other parts are worse since those parts are punished by long-term basis.

Long-term:
Failing races result in terrible long-term rewards because based on the race length, you will receive more or less worse punishments. If the race is short, we will receive less punishment for failing vice versa applies to when the race is long. If the race is complete: taking longer results in less reward than you would for completing in optimal times. Alike to what is currently written, long-term rewards focus more on how we should be rewarded or punished for how we have performed on the race?

Analogies for how cars will obtain rewards
Say at a certain time in a race, there are thousands of cars in a similar section. If you overlapped these, it would be absolute chaos. But if you also took the front cars versus the back ones, you’d find the front cars getting the higher short-term reward. But what if the all cars kept good pace with each other in comparison to race length, and the front cars fell off with end not far, in sight? This would give the previously-back cars good long-term reward. But what if instead of the front cars falling off, the back cars simply get a lead? Then the now, front cars will still get a better long-term reward than the now, back cars

How the types of rewards will be used
It has already been mentioned that the AI is given info on improvement but is actually that the AI is told how and where to potentially improve but is never told what to improve because it must figure out this on its own by natural selection and randomness. This section is dedicated to how the AI will use these rewards to mix in what I just mentioned and therefore, improving.

How the AI will evolve
Example
Example

Machine-learning types
Example
Example

Notes 

Explore new techniques created randomly by the AI
