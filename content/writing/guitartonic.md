---
title: Guitars + Programming = Guitartonic?
description: This was the day I was practicing my guitar, as usual. The warming up part is simple. I find a picture somewhere on the internet, let's say of a natural minor scale. Then I find a backing track on YouTube to play over that scale so it sounds less like I am in a music class and more like I am playing a solo improvisation.
date: "2024-01-10"
publishDate: "2024-01-10"
---

Armaan and I just shipped a [new product](/portfolio/guitartonic). It's called Guitartonic. Here's how it was born.

## Idea Genesis

This was the day I was practicing my guitar, as usual. The warm-up part is simple. I find a picture somewhere on the internet, let's say of a natural minor scale. Then I find a backing track on YouTube to play over that scale so it sounds less like I am in a music class and more like I am playing an actual solo improvisation.

![Natural Minor scale in position 4 in key G](/images/writing/guitartonic-1.jpg)

The problem with that approach is that it's annoying. I open the picture in one tab, then the video in another. Then the video ends and it auto-plays some random YT stuff. On top of that, the scale picture -- like the one above -- only shows the positions for a single key, in this case G.

Then the idea was born: I need to make positions random, and the keys random, and somehow still be able to pull music to play over it as a backing track. I quickly chatted with Armaan, and discovered that he had the same problem.

In 30 minutes, the first prototype was born. Meet Guitartonic v0.1

![The first version of Guitartonic](/images/writing/guitartonic-2.jpg)

While this didn't pull the music from YT (just yet!), and didn't show me the picture of the scale, it was useful because it made me jump over the whole fretboard instead of sticking to one position and playing in it for 5 minutes. The thing worked, but it needed improvements. Here comes the first proper MVP.

## MVP

I spent about three days of hacking this thing together. It is almost a joke at this point that all initial products take me at most three days to build. We even thought of launching a business called "Three Day MVP, Inc." to offer technical help to non-technical founders.

The MVP did everything that we wanted it to do. It had random keys, it had scales -- although basic --, and it showed the diagram of a fretboard. I even pulled some <a href="https://developer.spotify.com/documentation/web-api" target="_blank">Spotify API</a> to get the music going. Needless to say, it just worked.

![The first proper MVP of Guitartonic](/images/writing/guitartonic-3.jpg)

There started the most important phase of any product, and trust me, you should never, under any circumstances, skip it. The phase of user testing. I presented it to all my roommates -- not coincidentally, they all play guitar -- and ask them to spend 30 minutes to an hour each to play with it. Armaan did the same. That's how we got our initial feedback.

<br />

- "I don't have Spotify account" (most frequent)
- "Would be nice to have more scales!" -- oh, nothing can sink a product faster than a user's "would be nice". Learn to recognize which "would be nice"s are actually important to address, otherwise you'll end up building a "nice" product that nobody needs.
- "Position changes too fast"
- "Position changes too slow" -- jeez, people, did you see the "duration" slider? Oh, well, I guess I'll make it more visible.
- "Need to see more frets at a time" -- initially, I would only show the 5 frets of a single position

After a week or so of user testing, I went back to drawing board. I had to let go a few things, and add some others. I am also a minimalist of some sort, so I needed to redesign the whole interface and remove everything that is not essential.

Now, looking back at how it all started, the end product looked very much like the initial scale picture with the exception that I get to choose the key, and a backing track plays in the background. It was everything I wanted to have. It was perfect.

## The product -- guitartonic.com

![The website guitartonic.com](/images/writing/guitartonic-4.jpg)

The website was live. We removed Spotify and hosted backing tracks on the server. The tracks were of poor quality, but they did the job. We added some scales but still kept it pretty basic -- a few minor (pentatonic, blues, natural/aeolian), and a few major (pentatonic, ionian). We also added settings, so users could set their preferences if needed. This included note names, fret numbers, adjacent frets, and a playback time (kept at 30 by default). Now, not only everything just worked, it was also beautiful.

Over the next couple of weeks, we continued testing it with friends. We also launched it on Hacker News and Reddit, although with little success. In any case, we kept the tool online, and from time to time it still comes handy. I had personally outgrown it while I was building it. Because building it made me learn all scales in all positions. After all, that was the initial goal exactly =)

Guitartonic is online, and it is free, so if you happen to practice guitar, go give it a try!

https://guitartonic.com
