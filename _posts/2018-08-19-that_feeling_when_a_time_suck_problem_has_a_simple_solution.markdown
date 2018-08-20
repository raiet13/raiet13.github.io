---
layout: post
title:      "That Feeling When a Time Suck Problem Has a Simple Solution"
date:       2018-08-20 02:18:48 +0000
permalink:  that_feeling_when_a_time_suck_problem_has_a_simple_solution
---


Disclaimer: This is the second attempt for the "JS-Rails Project Blog Post". My first post ended up being about my project methodology and the dangers of Scope Creep, so I decided to keep that post for later. This post is about the two main issues that I ran into during the course of this project and that ended up being massive time sucks with incredibly "simple" solutions.

The first issue was that I was having significant issues with the active_record_serializer gem. No matter what I changed in the controller and js files, the JSON return was not displaying the expected format nor data. This "simple fix" was that I had accidentally copied the "active_record_serializer.rb" file in the config/initializers that was used for writing the serializer from scratch. That file was overwriting the default behavior of the active_record_serializer gem. Once that file was removed, the JSON render in the controller worked as expected.

The second time sucking issue ended up causing me to reach out to Project Support after painstakingly running through every line of code and running every google search I could think of yielded no answers. This ended up being a problem with adding new functionality to an existing project, where the "new functionality" wasn't completely different. As in, I *didn't* realize that my new code wasn't actually being called at all!

The root of this second issue has to do with the fact that I was using individual js files and therefore decided to go the route of adding a "yield :js" component to the main layouts/application file. Since the specified js files were only needed for the views in which they were being called, I added a "content_for" section only to those views. Since I was going back and forth through different views at different times, I was completely blind to the fact that the view causing the "code issue" didn't have the js file call. Such a small detail that caused me so much pain. 

On the flip side, I learned a lot about how to use the "yield :js" and "content_for" functionality. One thing that I learned is that when using this method of calling js files instead of using the js manifest(s) (i.e. javascript/application.js), each individual js file needs to be added to the pre-compiler in the config/initializers/assets file. Otherwise the js files won't be loaded properly.

Additional Resources Used
* [Learn Page Specific Javascript Lesson](https://learn.co/tracks/full-stack-web-development-v6/rails-and-javascript/asset-pipeline/page-specific-javascript
* https://api.rubyonrails.org/classes/ActionView/Helpers/CaptureHelper.html
* https://apidock.com/rails/ActionView/Helpers/CaptureHelper/content_for
* 
