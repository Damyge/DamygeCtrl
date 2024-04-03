+++
title = "My First CTF"
date = "2022-11-09T23:13:03.519Z"
author = "Damyge"
cover = "img/my-first-ctf.png"
description = "A cyber newbie describes his first CTF… heist movie style!"
tags = ['ctf', 'heist', 'story']
draft = false
+++

This is the tale of my first Capture The Flag (CTF) competition. Instead of a technical write-up, I’m telling this story heist style!

# The Job  
The North American Cyber Range Alliance and Grand University would be taking the CTF live at 09:00 in 9 days. The target would be a web site and its server, and I would have exactly 30 hours to get in, get root, and get the flag before the web server went down forever. On top of that, I had competition.

# The Crew  
It was going to be a tall order to do this on my own. As a beginner, I wasn't sure if I had what it took. But when I saw another newbie cybersecurity club member sign up, the inklings of a plan started to form. When I walked over and asked Red to team up with me he agreed. I wasn't sure we'd get higher than last place, but we were both going work hard and try our best.

# The Plan  
We didn't have much experience, but we did have a little time. I knew that it'd be difficult to practice compromising websites because there were too many unknowns about what the CTF page would be like. I had to count on figuring out how to get in once the competition started. But I also knew we'd need to take control of the server running the website once we were in, so I took a gamble. We dedicated all of our time before the competition to practicing privilege escalation to root the server once we got in. We just had to hope my gambit would pay off and we would be ready when the day came.

# The Suprise  
It came, alright, along with an unexpected surprise. Just an hour before the competition began, Red told me that another cybersecurity club member wanted to join us. I didn't know him, but I didn't see any problem so we brought Mark on board just minutes before the CTF started.

# The Entry  
The minute it started, we frantically started trying to learn everything we could about the website, prodding it for any weaknesses. On the outside, it looked like a regular Wordpress blog, but we needed to find out what was like on the inside. We started making good progress, and eventually, we took control of the admin dashboard! With that, we took the lead! Until...

# The Disaster  
We made a major mistake. We were messing with things we didn't understand and paid the price. The website went down, and so did the computer running it. I frantically contacted the organizers, and after a tense 15 minutes, they managed to bring it back online. Then we hit another roadblock: college classes. As I sat in class for the next two hours, I watched our competitors inch slowly closer to us on the scoreboard. When we got out of classes, we all rushed back to my dorm and set up our command post.

# The Finale  
Not long after setting up, we made our breakthrough. We used our control of the Wordpress dashboard to access the web server through malicious Wordpress plugins. Then, in rapid succession, we took control of every single user account on the system until we captured the most powerful entity of all, root. We used root to find and read the flag, and with that, we had won the competition with 20 hours to spare.

# The Getaway  
We closed our laptops with trembling hands and made our escape. We left our command post (aka my dorm room) and made our way on foot through our college campus to the nearest ice cream place, where we celebrated our victory.

<br>

If you got this far, thank you for reading. I had to keep details vague for this CTF because I know it is being reused, but expect future posts to go more in-depth on technical topics. Have a great rest of your day!