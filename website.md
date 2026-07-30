---
title: How I built this website
date: 2026-07-30
description:
unlisted: false
tags:
---
My personal site has [evolved a lot](https://www.param.me/notes/archive) over the years. This is the first version where I used any LLMs at all. Not only that, but I didn't really read the code at all. Some observations

With "vibecoding" I've noticed it's hard to lose intentionality in design. There are projects I've worked on since (like [param.me/poker-analytics](https://www.param.me/poker-analytics/)) where I give it a high level prompt, and an LLM generates a proposed design. There are many small decisions in between that are glossed over,  and even if I explicitly approve them, I never had to think through them from first principles. 

This site was not built like that. I was tremendously intentional with every part of the design, even more so than previous iterations where I was forced to code it myself. I found that vibecoding gave me the power to: 
1. **See a vision through.** I didn't have to compromise on a design I wanted because it was too hard or too time consuming. I didn't realize just how often I used to compromise on my original vision during the implementation until I was given the gift of an LLM. 
2. **Rapidly prototype different designs.** To really see how a particular design would feel, I previously would have to spend effort building it out. At that point, I would've sunk enough time into it that I would have grown attached to it. Or even if I wasn't, pivoting was costly enough that as long as I was sufficiently satisfied, I would stick to it. Now with rapid prototypes, I can be detached and find the perfect design I want 

Some examples of being intentional with the design:
## Timeline
In the timeline section, clicking on different timeline entries moves the map and cycles through photos. I wanted to make this feature discoverable, by making it easy to stumble into this. To do this, I made the map state change trigger as your cursor hovers through the timeline entries, without needing to click. And to make it even easier to accidentally stumble into this, I extended the hover hitbox to be the entire horizontal space to the right of the timeline entry, even outside the text. But this makes the hover effect too trigger-happy, such that once you've selected a timeline entry, you might accidentally trigger another timeline entry. So I made the hover hitbox shrink to just the width of the text when you have an entry selected. If you have nothing selected, the hover hitbox remains extended so users can discover this feature. 

## Dark mode
I see a lot of personal websites with a dark mode. I was really hesitant to add dark mode to mine, because I've designed the site in a very opinionated way. While it is minimalist, it's exactly the way I want it to look. When you're on my personal website, you get to look at what I made and my design choices. Originally, I had no dark mode. I only added it because of this notes section I later added, which I think would be too cruel to force people to read in light mode. (I want to be able to occasionally write standalone blogs that can be read by a larger audience, who don't necessarily care about me or my design choices. I added it as a purely utilitarian feature for them.) And I hate the inconsistency of only having the dark mode toggle on the notes page. 

Still, I want dark mode to just be there only if you're truly inconvenienced by light mode. You should always see my website in light mode the first time you open it, then you're given the choice to switch. So I deliberately didn't set my site to use the system dark mode settings. One of my friends even brought this up to me. I was somewhat surprised that someone even noticed, and I was glad to share my thought process behind this very intentional choice. 
