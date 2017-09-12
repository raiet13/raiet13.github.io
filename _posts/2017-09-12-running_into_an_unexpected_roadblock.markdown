---
layout: post
title:  "Running into an Unexpected Roadblock"
date:   2017-09-12 02:04:59 +0000
---


This lab was surprisingly difficult given how easy the labs leading up to it were. The requirements through the r_spec tests were relatively straight forward, but there was an interesting disconnect when it came to execution. When translating the pseudocode into real code, everything appeared to make sense from a logical standpoint, but the functionality was surprisingly inconsistent. Code that would work for several requirements would fail for others. It appeared to be relatively random and therefore made debugging quite difficult. 

Given that the spec simply detailed the input used for the test and the expected output of the test, it was very hard to pinpoint exactly where the code was breaking. As the code was broken up into functions (known as methods in Ruby), it seemed like it should be relatively obvious to determine which function(s) were causing the errors. However, the functions themselves were quite entwined, causing supposedly straight forward code to act erratically. It was particularly confusing when certain outputs would register as passing the tests, while related outputs would act completely opposite. 

For example, the "won?" method would cause the "diagonal win" to pass, but then using the "!(won?)" functionality would cause the "diagonal win" to still pass. Perplexing right? Especially unhelpful when the test essentially (and simply) states "expected false value but received true value".

As a programmer who is used to being able to add as many print statements (also useable as "puts" in Ruby) into code for pinpoint accuracy about code breaks, the biggest struggle I had with this lab was the lack of code execution. I had to rely solely on the r_spec outputs rather than running the code in a testing environment with the print statements allowing me to identify just *what* was being digested by the code at any given point in time. 

Though I didn't end up using "Ask a Question" right away, I did see parts of code that another student used, and the back and forth that was had in regards to it. It was being able to see the other student's code that really helped me figure out broken pieces of my own code. Personally, I find it too bad that there isn't a solution code repository. I've discovered that, at least for myself, at some point, the easiest way to learn about the deficiencies in personal code is to see a working solution. When accompanied by an explanation of *why* the code is laid out the way it is, and why it works, solution code is the best thing ever. 

This lab is certainly the hardest lab thus far, and quite frustrating! 

**Update** : I eventually caved and "asked a question". One screen share later with a tech coach, and I learned that the pseudocode from the lesson was actually leading me down the wrong path! I was correct in regards to *where* the issue was, but my reliance on the given pseudocode example made it hard to see just *what* the issue was. The pseudocode put the "else false" section within the "win_combinations" loop, but the "false" actually belonged outside of that loop. A simple change that made sense once the tech coach pointed it out. I won't say that I will definitely jump to "ask a question" in the future, as I still want to struggle with fixing the code on my own, but it was definitely worthwhile! This was nearly a "pulling hair out" situation haha.


