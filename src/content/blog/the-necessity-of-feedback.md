---
title: "The Necessity of Feedback"
description: ""
pubDate: 2025-07-30
tags: ["feedback", "demand survey"]
---

I completed the MVP of my first app and shared it with two friends to get some feedback.

I didn’t ask for specific improvements or changes from the beginning—I just showed it to them raw because I wanted to see their unfiltered reactions. After all, their initial impressions would likely reflect how most people feel when they use the app for the first time.

After lunch, we went to a nice café near Konkuk University. I showed them the app installed as an APK on my phone.

Even though they were close friends, I felt a little nervous—and honestly, a bit awkward too.

<br>
Their feedback could be summed up into five main points:

- Improve search speed
- Make the source and target languages easier to identify at a glance
- Allow same-language searches (e.g., English to English)
- Change the font of the app’s title on the main screen
- Modify the app’s background color

<br>

First, there are two ways to improve the search speed.

One is upgrading the GPT model. Initially, I planned to support faster searches through a paid plan. But at the current speed, users may already feel frustrated on their first try—something that could easily lead to drop-offs.

The second approach is to switch the response format from JSON to Markdown. JSON includes a lot of brackets and indentation, making it less suitable for fast responses. I initially chose it because it allows more control over structured data, but it turns out parsing takes longer than expected. Considering the current level of output, Markdown should work just fine.

Making the source and target languages easier to understand was something I had worried about even before. No matter how clearly it’s explained in a tutorial, I wasn’t sure if a first-time user could grasp it right away—and that concern turned out to be valid.

I’m also considering whether it's even necessary to ask users to select both source and target languages. There may be a better solution out there.

As for same-language searches—wow, I hadn’t even thought of that. Even native English speakers look up unfamiliar words in English-English dictionaries. I had fallen into the trap of thinking nuanced meanings are only relevant when translating between languages. This is definitely something I’ll fix right away.

The last two points are about design. Personally, I thought the title font looked fine (I did choose it in about 15 minutes, but I trusted my taste). Still, both friends said it looked outdated.

For the app’s base color theme, I went with a light beige to avoid a traditional “dictionary” feel and give off a softer, friendlier vibe. But one friend said it looked dull. When I asked for more insight, they explained that if I want to keep that tone, I should go all-in with that concept—or remove it entirely. Right now, the background is beige while the rest of the app is clean, which makes the screen feel a bit murky. I could see where they were coming from.

For the design side of things, I plan to reference other well-designed apps and try replacing some of the colors.

<hr>

What I took away from this feedback session is simple: I need other people’s eyes. Fast development, fast feedback, and fast iteration—this is what matters most. And ideas that come from things I hadn’t even considered? Those feel like discovering hidden treasure.

I’ll quickly work on these changes, release an update, and gather more feedback from real users to keep improving the app.
