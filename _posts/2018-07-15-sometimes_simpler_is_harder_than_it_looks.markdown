---
layout: post
title:      "Sometimes 'Simpler' is Harder than it Looks"
date:       2018-07-16 01:56:57 +0000
permalink:  sometimes_simpler_is_harder_than_it_looks
---


After working on the Sinatra project and blazing through the rails section, it seemed like this project would be completed in a matter of days tops. Ignoring the personal issues that occurred between starting the project and completing it and my usual inability to come up with a satisfactory idea, there were a few technical parts that were less obvious than expected. That especially applied to coming to a strong realization about the importance of coding environments, why testing consistently is key, and understanding communication systems.

To keep this blog post simple, I'm just going to hit each of the points listed above with the main pain points and resolutions. Though not right now, I hope to flesh each point out in later blog posts geared specifically to the challenges and resolutions that I encountered. Each of them does relate to the rest, at least in the scope of how and why I struggled with this project, but they can be unpacked further and were more or less resolved individually.

- - - - - 

Firstly, as someone who has several different coding programs for various languages and purposes on my computer while also using it for personal use, I eagerly took to using the Learn IDE. It was nice to have an isolated environment where I didn't have to worry about any installations that could possibly change previously altered settings or cause complications with any of those other programs. Adjusting to using the IDE was simple, and definitely helped me focus more on the coding aspect of my learning. 

However, when I was mid-project and the IDE suddenly stopped working, I realized that I didn't truly understand how the environment worked, and that the basic restart or reinstall and trolling the FAQs weren't resolving my issue. I eventually caved after some excessive searching, and set up a Project Coding Meeting. It was there that I learned that the IDE wasn't meant to be continued post-Sinatra and that the fact that my IDE did work for as long as it did was a fluke. 

Apparently most students ran into the issue much earlier than I did and brought it up in a time when "Ask a Question" was a possible resource. My solution to this problem, switch to C9 (a really great development environment that is completely cloud based).

- - - - - 

Secondly, I learned that testing at every point throughout, no matter how confident you are in what you are coding (ex. if it was working earlier and tested in previous labs). Usually, I test as much as possible. Once I've made an adjustment that should cause some sort of change, I test it. That way I know if my modification worked or not. That was how I started the project, up until I suddenly couldn't test any further due to environment issues (see issue one).

Unfortunately, my confidence and understanding of the material did me absolutely no favors. Before I made the switch to C9, I was determined to at least finish what I expected the project to end up being. I didn't want to waste time and believed that the code made logical sense so it should work properly. This was a mistake. That is not to say that the code I wrote was actually wrong. I am happy to report that I didn't end up having to scrap all of it because it wasn't working properly. However, that doesn't mean that I made the correct decision in putting off reaching out for help with my environment while continuing to code.

The resolution here was that I discovered, after I went through the strenuous and time consuming process of migrating all of my code over to C9, that I had to do a lot of fixing and adjusting because the code that worked due to the nature of the Learn IDE did not work with the C9 environment. That meant that I ended up having to adjust most of the code to reflect the new structure and delete other bits that were suddenly obsolete. If I had stopped coding to prioritize diagnosing the lack of testing and thus made the migration sooner, I probably wouldn't have wasted my time on code that was no longer relevant.

In conclusion, testing is important! When it comes to ensuring that a project is progressing properly, it is definitely important to make sure that testing is possible at every hurdle. Otherwise you can end up like me and do unnecessary hours of work.

- - - - - 

Thirdly, understanding the communication systems in place for the project are just as important as the environment and coding. In the Project Meeting that I had, and mentioned by my educational coach, apparently there should have been an email alert that was sent out once I passed my Sinatra Project. This email alert was supposed to have let me know about transitioning from the IDE to a "local environment", thereby avoiding the situation entirely.

Unfortunately for me, I didn't see the email. I'm also not entirely sure that it would have proven helpful given that I was mostly done with the Rails section before I had my Sinatra Project review, but that's a different story. Regardless of the circumstances, I had the expectation that important information would be transmitted to me through the web platform, either through a read-me or lab. This was a mistaken assumption. Though some important alerts and notifications are clearly marked in read-mes and labs, Learn sends out email alerts for other things.

In conclusion, when starting a project, it is important to identify communication strategies and systems. To know what to look for and what to expect. Moving forward, I will definitely be paying closer attention to the emails that I receive from Learn and checking it more frequently.

- - - - - 

Finally, I just want to conclude that I definitely learned a lot by working on this project. This blog post isn't quite technical as I believe that the main technical challenges I faced might be better off fleshed out in subsequent posts, but I will list a few here.
- Migrating from the Learn IDE to C9 Environment
- Using OmniAuth for Google and creating BOTH a local and a third-party login/signup system
- Using nested resource routes ONLY for certain routes (index/new/edit) but NOT for others (create/update/destroy)
- Constantly changing and updating my base idea while trying to navigate and fulfill each of the spec conditions

