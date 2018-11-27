---
layout: post
title:  "I Git in Trouble"
date:   2018-04-02 02:00:00 -0600
categories: programming
comments: true
---

Wow, that was a journey through git that I never want to experience again. Faced both with my own stupidity, git bugs, spotty internet, and a late-night screwup, I don't know what else could've gone wrong for me; except for losing this blog entirely. 

![github](https://upload.wikimedia.org/wikipedia/commons/e/e0/Git-logo.svg)

I was faced with a huge problem, and I decided to just get some words down the same night to narrate my thoughts and mistakes, so as to not be repeated. This opens me up to bad writing and/or egregious mistakes, but at this point, I'm just ecstatic that I came out of this situation intact. This is definitely going to be a memorable moment in my web development journey. 

This all started with me cleaning up my files late at night. I looked over my documents folder and went about cleaning it up, renaming files and folders, as well as filing things away that weren't needed. Upon seeing the name of my personal blog being misnamed, (from back before it was my user page and just a project page) I was irritated and changed it from sidhant-blog to sidhantmathur.github.io. If not for this mistake, I could actually have gotten a decent night's sleep, but alas it was not to be. I made the name change, changed the previous sidhantmathur.github.io to its current repo name: bootstrap-port, and then went to push the changes. I saw that there were 300+ files to be changed in my blog's repo, but I thought nothing of it; it was probably just that renaming a repo required all the files to be moved into a new folder. Unfortunately, the reality was that my blog and all it's contents were replaced by my old portfolio. 

My heart started racing as I thought that all the work on the minutia of the CSS and all the written blogs were gone. Luckily I soon found that they weren't, however, the website had problems because jekyll and github pages were no longer installed correctly. I had to fix this whole mess at once. I searched through many old blogs and stack-overflow posts giving tutorials on how to undo a forced push so that I didn't have to go through the process of reinstalling jekyll and github pages in the same way. I eventually found my way to the problematic commit (even though commit history is deleted upon a force push, it is still retained at 

```https://github.com/repoowner/reponame/commit/master#{OLD_SHA}```

However, getting the commands correct to revert was a bit tricky, especially since my internet at the time was spotty (making it difficult to know whether a git failure was a bug, me, or the internet), though it was eventually done. All I had to do was force push the reversions to the origin. This however scared me a lot, because of my experience with force pushing so recently going horribly. I had learned a lot of obscure git commands in just a few minutes, and yet I felt terrified of one of the more basic and necessary ones; unreasonable I know. 

![SHA](https://upload.wikimedia.org/wikipedia/commons/e/e2/SHA-1.svg)

What I found from this is that I am not the only one who has faced this issue, and I am also alarmed by how problematic using a visual git manager like on Visual Studio Code, as well as Git Bash together can be if you do not pay attention. Miscommunications or unfamiliarity with one or the other can really screw up your day like it did to mine. Late night git force pushes aren't something I will be trifling with again. 

### Update

Since writing that "I won't be trifiling with git late at night," I continued doing just that, fixing the file system, trying to remove residual git trackers, and I don't think I will learn my lesson easily. 

I ended up reforking jekyll-now and manually making most of the changes back to normal. Thankfully it's all over. 