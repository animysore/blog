---
layout: post
title: "Why video games should get better security"
description: "Here's what happens when you hack a mobile video game"
modified: null
tags:  
  - video games
  - hacking
  - nimblequest
image: 
  feature: "matrix-2.jpg"
  background: "matrix.jpg"
comments: true
share: true
published: true
---

***Here's what happens when you hack a mobile video game***		

Last week, I downloaded Nimble Quest, a game inspired by the Nokia classic `Snake`. The game itself is quite fun, featuring about 16 playable characters, of which one you need to choose as your 'Hero'. There are an unlimited number of levels, each with a number of enemies your character needs to kill. As the game progresses, more characters line up behind your Hero to form a chain. The characters handle all the killing on their own, and your job is to make sure the Hero does not collide with enemies or walls. 

After a few minutes of playing, I got curious and loaded up the file manager on my phone. I located the game's `Data` folder, and opened up the preferences' `xml` file. 

<figure>  
    <a href="/images/games-datafolder-path.png">
        <img src="/images/games-thumb-datafolder-path.png" alt="">
    </a>
</figure>

Hacking the game couldn't have been easier. Values of Unlocked characters, gems and coins, powerups, everything. They were all stored in an easily readable format. I just played with some numbers, and this happened. 
  
{% highlight bash %}
<int name="gems" value="19191444" />
:
:
<int name="powerup_bomb" value="5" />
<int name="powerup_shield" value="5" />
<int name="powerup_attack" value="5" />
:
:
<int name="crystals" value="799919" />


{% endhighlight %}

In the end all my geeky knowledge helped me to hack into the game (in about 20 minutes), resulting in this :  
<figure class = "half" >  
	<a href="/images/game-init-screen.png">
       <img src="/images/game-thumb-init-screen.png" alt="">
    </a>
	<a href="/images/game-finl-screen.png">
        <img src="/images/game-thumb-finl-screen.png" alt="">
    </a>
</figure>   

All the cheating finished, I settled back, to enjoy the game. It was fun for the first 10 minutes or so. I could handle everything the game threw at me. I could purchase an unlimited number of `retry's`, which basically meant I was Invincible. Without the difficulty challenge however, I lost all interest after a few rounds, and stopped playing.  I suddenly realized a great universal truth. <i class="fa fa-lightbulb-o"></i>

>Hacking the game, had made the game *less* playable and *less* fun. 

I completely gave up on trying to play NimbleQuest and wondered if other games would be this easy to hack. My curiosity got the better of me, and I downloaded three more games made by the same game developer Nimblebit. 

***Every single one*** of those games had the exact same gaping hole in their security. All I had to do was change an `xml` file to bend the game to my whims and fancies. Even the file `path` for storing critical game info was exactly the same. None of the games had any backup, or any sort of web-synchronization to prevent me from hacking their data files merely by changing a few numbers. It was as if the developers WANTED everyone to do this. 

The greatest irony, is that developers who rely on in-app purchases for a no small portion of their income, are either too lazy or too ignorant to design better security measures. Why is it, that anyone with a little know-how about apps, can easily hack these games? And its not always the small developers that are to blame here.Even some of the largest game studios' on Google Play, make games which can be hacked by a child who knows to use a file explorer. NimbleQuest for example is a game with a ***million*** downloads on google play. They offer in-app purchases ranging upto $25 (nearly 1600 Rupees on the Indian version), for different coin and gem packs. Surely they would be upset if everyone suddenly stopped buying their IAP's and hacking the game instead to get a higher score. Yet it's as if their security is non-existent, trusting only on their users' ignorance to keep their money flowing in. (Which by the way is a not a completely bad idea, given that very few people would take the time to learn how to and then hack a video game) 

Now I'm not saying this whole game-hacking issue is something limited to android, or even the smartphone-age. Video games have been hacked from the time they've been around. The big difference, is that *Freemium* games, which ask you to pay money to progress onward in the game more easily, have almost always been completely internet based, or heavily encrypted when playable locally. Its only since the smartphone explosion that these games are being made for offline use too. Now the idea behind a freemium game is that either you use your skill to become better at the game, or you pay to receive extra benefits which help you as the game's difficulty increases. Personally I feel freemium games should be banned, as it creates a divide among gamers - those who can play versus those who can pay - and transforms a video game into a mini-virtual-shop. And the fact that most of these mini shops have virtually no security, thieves can easily target them, effectively breaking down the whole 'economy' of the video game. By making it easy for hackers, game developers are being unfair to the others, especially the people who like pay to purchase a coin bundle. 

Summing up, I would like to say that freemium games ought not to be hacked because chances are, it will inconvenience a lot of people. I would also like to warn those who want to hack a freemium game, that the results are not what you would expect.I can assure you, playing a video game within the rules set by the developers is ***much more fun than overriding that directive and going god***. 
