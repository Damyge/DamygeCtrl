+++
title = "The .Zip Disaster"
date = 2023-05-18T23:00:55.977Z
author = "Damyge"
cover = "img/google-zip/gz-cover.png"
description = "Comments on Google's new .zip domain and my PSA project"
tags = ['zip', 'google', 'web']
+++

Earlier this month, Google's new Top Level Domain (TLD) launched, allowing websites to now host on .zip addresses. Instead of *mywebsite\[.\]com*, it can now be *mywebsite\[.\]zip*. This can be a bit annoying because .zip is now both a TLD and one of the most common file types. But it can also be **dangerous**. Let's see an example in action:
<br>
<br>
![Demo: Family Photos](/img/google-zip/familyphotos.png)
<br>
As you can see in this demo, Matt tells his family "Check out familyphotos\[.\]zip" and the file name is already highlighted. If you did not understand that .zip is also a domain now, you would easily assume that clicking that button would allow you to access that zip file. However, When clicked, a HTTPS request is made to the domain https:\\\\familyphotos\[.\]zip and a zip file is downloaded without even opening a web page. This zip file can then contain anything the domain host wants it to (a text file in this case).

Let me break this down in more detail:
1. Software that automatically converts the text of links into a clickable hyperlink will now convert any reference to a .zip filename like "test\[.\]zip" into a clickable hyperlink unless programmed specifically not to.
2. Scammers and phishers can abuse this to create malicious .zip domains which download malware, enabling untechnical users to click what they think is a zip file (ex: test\[.\]zip) which downloads a file of the hostile actor's choice instead.
3. Using this method, malicious actors can now host malware on domains of common filenames like "backup\[.\]zip" and then just wait for unknowing users to click on links pointing to what they thought were zips.

How can we respond to this? There are two big takeaways. First, if you are a network admin, ban the entire .zip TLD from being accessed on your networks. If you are a regular user, do not visit .zip domains given they are now a wild west for hosting malware.

Finally, if you found this post useful, [please connect with me on LinkedIn](https://www.linkedin.com/in/dylan-ierley-28a9aa24b/). I'd love to expand my network and see that this resource is helping people.