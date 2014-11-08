---
published: false
---

## What happens when you hack a mobile video game		

Last week, I downloaded Nimble Quest, a game inspired by the Nokia classic `Snake`. The game itself is quite fun, featuring about 16 playable characters, of which one you need to choose as your 'Hero'. There are an unlimited number of levels, each with a number of enemies your character needs to kill. As the game progresses, more characters line up behind your Hero to form a chain. The characters handle all the killing on their own, and your job is to make sure the Hero does not collide with enemies or walls. 

After a few minutes of playing, I got curious and loaded up the file manager on my phone. I located the game's `Data` folder, and opened up the preferences' `xml` file. Hacking the game couldn't have been easier. Values of Unlocked characters, gems and coins, powerups, everything. They were all stored in an easily readable format. I just played with some numbers, and this happened. 

{% highlight bash %}
├── data
|    ├── data
|    |   ├── com.nimblebit.nimblequest
|    |   |    ├── files
|    |   |    ├── shared_prefs
|    |   |    |    ├── com.nimblebit.nimblequest.xml
|    └── 
├── sdcard0
├── sdcard1
└── system
{% endhighlight %}


