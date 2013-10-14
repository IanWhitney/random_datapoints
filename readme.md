# Random Dataponts

This is a tool to store, track and visualize anything that you care to track and visualize. Well, almost. Want to enter your weight each day and see it visualized as a line graph? Sure. Want to track the amount you spend on coffee each day? Ok. How about a list of movies you watched? Sure. Want to do anything complex? Then this probably won't be useful for you.

## Getting Started

- Clone this project
- `bundle install`
- `rake random_datapoints:install`
- `rails s`
- open http://localhost:3000/
- Follow the directions on screen

## Under the Covers

Random Datapoints is a web app built using Ruby, Rails, Redis, Ember and D3.
Ruby powers Rails, Rails serves up your data, Redis perists your data,
Ember handles the Web application and D3 handles the visualizations.
There's other stuff in there, but those are the major components.

## To heck with Ember and D3, can I get my data directly?

Yep. Ember and D3 are just sitting on top of a restful API providied by
rails. Say you're tracking your weight and you wanted to see that raw
weight data in JSON format:

    /data/weight.json


