# How to _not_ be a dinosaur.

This is the story of how I became an experienced senior frontend developer and how I had to start all over again. How it *felt like* I had to start all over. How to learn. 

This story is mostly about learning React, but might apply to other frameworks as well. Heck, it might even apply to completely different areas of expertise.

## What happened? 

It is 2019 now and I am 37 years old. I have been working for 15+ years professionally as a web developer and web designer. After highschool I went to design school and learned to be a designer. But I have also always been interested in coding. In the early 90's I was already writing code in [GW-Basic](https://nl.wikipedia.org/wiki/GW-BASIC). I can recall writing my first lines of code in the last grade of primary school. Later I learned HTML and even a little PHP 3. In design school I also learned Flash and OOP in [Lingo](https://en.wikipedia.org/wiki/Lingo_(programming_language)). When my class got the task to code a simple dice rolling program, I wrote the complete Monopoly game. Just because writing code was a never ending path of discovery, wonder and [dopamine](https://www.npr.org/sections/ed/2014/10/24/357811146/curiosity-it-may-have-killed-the-cat-but-it-helps-us-learn?t=1572532599814).

![](https://raw.githubusercontent.com/MyOnlineStore/blogs/Dinosaurusblog/public/johan_old.png)

_This is not me. But it could have been if I had such an awesome mustache at the age of ten_

In the years working as a developer I have seen the landscape around me change drastically. When I started designing and coding in the early 2000's, CSS, some javascript and later jQuery was all I needed to master being a frontender. I also added some backend code (PHP and even Coldfusion in a dark era) to be able to integrate your frontend code with the backend. So for years I could design a project, code it and integrate it. At one point I was named a full stack developer. Life was simple. Even simpler when post processors like SCSS came to life. I was like "I got this, bro!"

![](https://raw.githubusercontent.com/MyOnlineStore/blogs/Dinosaurusblog/public/johan_happy.png)

_Also not me._

## So what changed?

So I was happily writing SCSS, JS and some PHP, but then around 2012 the world started to change around me. I saw more and more articles about fancy frameworks like AngularJS on Twitter. At some point it seemed like new frameworks were being released every day. I was naturally drawn to this, but couldn't keep up and got a little overwhelmed by the seeming complexity of some of these frameworks. And I also suffered a bit of [metathesiophobia](https://www.fearof.net/fear-of-change-phobia-metathesiophobia/).
  
![](https://raw.githubusercontent.com/MyOnlineStore/blogs/Dinosaurusblog/public/johan_worried.png)

_Still not me._ 

Then one day I attended a meetup where some guy enthusiastically demonstrated AngularJS. He made a list of hospital employees which could be clicked to unfold a list of their certifications and skills. A very simple page. And the amount of code that was shipped to make this simple page work was over 1mb.

So that was it for me. This new stuff was overly complex, scary and most of all: I could write this accordion list in less than 1kb of vanilla JS. Or maybe even without JS in CSS and HTML only… My common sense said: "Why the **** would you use something _so_ complex for something _so_ simple?!"

![](https://raw.githubusercontent.com/MyOnlineStore/blogs/Dinosaurusblog/public/johan_wtf1.png)  

At that time I was the only frontend developer at [MyOnlineStore](https://www.myonlinestore.com/). And I have always been the only frontend developer for all my previous employers. So there was nobody to convince me that it would be wise to embrace these new techniques.

## Why I stood still for so long

In late 2015, when I was already late to the party I got sick. A severe burnout followed by a big relapse one year later while I was still recovering. When I felt a bit better after a while and came back to the [MyOnlineStore](https://www.myonlinestore.com/) offices everything had changed. There were two new frontend developers. With new repos, new code, new words, new everything!

![](https://raw.githubusercontent.com/MyOnlineStore/blogs/Dinosaurusblog/public/johan_wtf2.png)
  

It was 2017 already. I did not know where to start. I didn't dare to ask for help, because of my misplaced pride. I was writing code before some of my new colleagues were even born… and now I should go to these guys and admit I had no clue what I was doing?

But I tried… I tried to keep up with it for a few months and then I was like: "I don't get it! fuck this shit!" 

"I have been doing design _and_ development 50/50 for all of my career, so now it's time to say goodbye to one of these and focus on the other." And since I got _so_ scared of The New Frontend World, I fled to the design department of [MyOnlineStore](https://www.myonlinestore.com/). This was in early 2018.

![](https://raw.githubusercontent.com/MyOnlineStore/blogs/Dinosaurusblog/public/johan-drawing.gif)

_Yes, this is me doing design_

Unfortunately, after a year of doing (UX) design, I found out this was the wrong choice. After years of intensive therapy and running straight into a black hole that was another potential burnout, I came to the conclusion that design was not for me. I am able to design, but I can't handle the stress that goes with it. I felt like I had to answer and fight for all the design choices I made. And since my UX designing was mostly driven by instinct, this was really hard for me. On top of that it all felt very personal. Maybe I can handle it today or in the near future, with all the things I have learned since, but not then. It fueled my insecurity enormously.

And then in late 2018, I decided to go back to frontend development. There I was, a frontend dinosaur in a modern world.

![](https://raw.githubusercontent.com/MyOnlineStore/blogs/Dinosaurusblog/public/johan_dino.png)

_Yes this is me._

## How to get up to speed? 

Now I faced a big challenge. I didn't want to go extinct like a real dinosaur and stick to my old habits, so how do you get up to speed after being paused for a few years in a world that changed (and is still changing) so rapidly? The first thing to overcome was my aversion for The New Frontend World™️. I tried to look at React and all other new tools with a fresh and unbiased view.

While I was away in design world a lot has changed within our codebase, but also in The New Frontend World™️. The tools we used improved or were replaced with better alternatives. The tools and codebase became more solid and mature.

Then there was news: [React Hooks](https://reactjs.org/docs/hooks-overview.html#%EF%B8%8F-effect-hook) was about to be released in React 16.8. This made code _so_ much more readable that I started thinking "Hmm, maybe I can do this".

I don't want to go all geeky on the differences between hooks and classes and why hooks are so awesome, especially since there are many [excellent](https://reactjs.org/docs/hooks-intro.html) articles [written](https://itnext.io/whats-the-big-deal-with-react-hooks-d73145eb14e0) on this [subject](https://medium.com/frontmen/react-hooks-why-and-how-e4d2a5f0347). If you ouwld like to learn more about this, you should check [them](https://reactjs.org/docs/hooks-overview.html) out.

For me personally the biggest thing was the improved simplicity of using hooks in function components compared to using class components. Where it felt like class components made me jump through hoops to keep track of of state, hooks just let me use [`useState()`](https://reactjs.org/docs/hooks-state.html).

For example, in oldskool classes, I used to write this to increment a counter:
```javascript
this.setState({ count: this.state.count + 1 })
```

Where hooks let me do this:

```javascript
setCount(count + 1)
```
I bet that if you are reading this you'll feel that the second version is simpler even if you have little (react) programming experience.

After this "challenge accepted!" point the hardest obstacle had to be overwon: how to handle the "I have to start all over again" feeling. I felt like I knew nothing. I was Jon Snow.

## Dealin' with dem feelins...

Who had I been kidding all these years calling myself a senior developer? How embarrassing was it that I had to ask my 12 years younger colleague for help over and over again...  

![](https://raw.githubusercontent.com/MyOnlineStore/blogs/Dinosaurusblog/public/johan_knowsnothing.png)

Some people will think "what's the big deal?", and I am happy for you if you do, but you have to understand that asking for help was a big issue for me. And a major cause for my burn out and the personality disorder that came with it.

So I did two things: I decided to start learning all these new tools and frameworks and more importantly I started to ask for help. But the most important thing I did: I told my colleagues how I was feeling and how insecure I was about everything. They were very supportive and this gave me the confidence to go for it.

One of the most supportive things they did is showing me that I did make progress. A lot, actually. They also showed me that not knowing everything is not the end of the world. As long as I you keep trying and learning, things will work out in the end.

Soon, I also realized I did not have to start all over again at all. It might have felt like it, but I still had a big headstart with my years of experience in programming overall. It was just a new framework and new tools that I needed to learn, not learning how to speak and not the first tool I ever used.

It will take some time to learn all these new things. And that's okay. Good things take time. I should have realised this earlier since it's litteraly written on my body, but sadly it's not that obvious sometimes.

![](https://raw.githubusercontent.com/MyOnlineStore/blogs/Dinosaurusblog/public/johan_arm.png)

_Yes, this is also me._

## Okay great, challenge accepted! Where to begin?

First I made a list of all the tools we use. There were quite a few things for me to learn: Typescript, Babel, Webpack, React, Apollo, Redux, GraphQL, Yarn and many more. This list was somewhat overwhelming until I started to put them into two groups: things I needed to learn right from the start and things I could figure out later. It turned out the first list is not that big and and a lot more do-able.

For example: I now know how to set up a project using Babel, although I have no idea about the inner workings. And that's okay, I will learn it some day. Until then it's perfectly fine to ask a colleague who does get it.

Bottomline is that it is okay to not know things. It's not the amount of things you know that make you a senior developer, it's the way you handle things [that make you a senior](https://medium.com/better-programming/how-to-be-a-good-senior-developer-958948e02ada). In my opinion.

I have always tried to take some time for personal growth once in a while, but this was only a few spare hours every now and then. However, since a few months our company [MyOnlineStore](https://www.myonlinestore.com/) is doing so called [Ship-it days](https://www.atlassian.com/company/shipit) where we developers can do whatever we want as long as it's somehow work related. This is a great way for me to learn stuff I might not naturally learn during everyday work. When I work in our normal codebase I just run `yarn dev`, storybook starts and that's it. But on these ship-it days I create new repo's, install packages and configure everything myself. That is a great way to learn new things.

## Conclusion

Take your time: good things take time.

Be yourself. 

Be awesome. 

---
If you liked this blog, please let us know by giving us some claps, retweets or likes.

If you think working at MyOnlineStore would be something for you, here are our [job openings](https://www.mijnwebwinkel.nl/vacatures) (NL).

If you have questions about this blog check out what I do in my spare time or just want to get in touch, you can find me at [Bad Decision Works Instagram](https://www.instagram.com/bad_decision_works)

You can find more of our blogs on [Medium](https://medium.com/myonlinestore) 

Cheers 👋 