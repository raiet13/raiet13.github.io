---
layout: post
title:      "The Trials of Getting a Kingdom Up and Running"
date:       2018-05-24 01:54:48 +0000
permalink:  the_trials_of_getting_a_kingdom_up_and_running
---


Entering into the Sinatra project, I was confident that it wouldn't be that hard. I think I've actually started dreaming about Activerecord and the MVC structure. Not surprisingly, the first hurdle I encountered had absolutely nothing to do with coding and everything to do with "what the heck should I code?". I am pretty sure I spent at least half of my overall time spent struggling with that.

When I decided what I wanted to do, I thought that it would be too simple, so I made my idea more and more complicated. My idea was to create a "user library" along the lines of Amazon or other multi-purpose websites. The basis for this idea was to take everything that I was working on previously and have it culminate in this project. Therefore, the basis would be that "users have playlists" and "playlists have various objects". So this "user library" would have music playlists, like iTunes, and book collections, like Kindle, and playlists of movies that the user wants to watch, like Netflix. For each of these playlist associations, there would be further associations like the Song/Artist/Genre and the Book/Author/Genre, and etc. Of course I would include data like "year_released" and "time_length".

However, the more I thought about how to structure this app, the more complicated it became. Before I knew it, I had absolutely lost sight of what I was meant to be doing. I felt like my head was going to pop off. I started writing diagrams, then scribbling all over the paper or tearing it up. I then took a breather and binge-watched some of my favorite youtube let's player. If there is one thing I've learned throughout my years of coding, it's that sometimes you really need to just take a step back and take a break. Fortunately for me, this break ended up inspiring me because the youtuber I watch, Olizandri, happened to be playing "Ni No Kuni II: Revenant Kingdom".

Extracting the main parts of the game that I felt were directly relevant, I boiled my associations down around the "user" model, which would be the "player". The associations then became "kingdoms", "citizens", and "outfits". Once I decided on those 3 additional models, the rest came swiftly. I checked off each requirement as I figured out how the associations made logical sense along with them.

Once the backbone of the project was set up, the coding was not as challenging. The only time I got really stuck was during a bit of very useful code from the complex forms associations lab. This bit of code caused checkboxes to be checked or not checked based on if the main object had the associated objects or not. In the case of the complex forms associations lab, that would be if the owner had the pets or not. The problem with diagnosing the code was that it was a bit of code that was never fully explained in the lab, so every search parameter I used didn't get me the information I was looking for.

I turned to Learn for help but ended up getting redirected a few times and waiting. Luckily, it was such a small bit of code that I could continue without fixing it right away. Ultimately, I found my salvation in the Sinatra Slack room, where someone explained the issue with the code to me. The additional bit of code for the checkbox logic needed to be INSIDE the first input tag.

The second issue I came across was that "type" is NOT a good value to use for migrations and models. I forget the exact reason why, but it is the way "type" is handled. The fact that there are a list of values that should be carefully observed is definitely something I will remember moving forward, as it definitely helps with identifying the source of database related errors.

Overall, an interesting lab to complete.

