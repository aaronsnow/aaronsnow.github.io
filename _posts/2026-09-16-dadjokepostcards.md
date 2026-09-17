---
layout: post
title:  "Weekend AI Learning Project: Send a Dad Joke on a Postcard"
date:   2026-09-16 00:00:00 -0400
# categories: dadjokes ai development
---

Hey, I made a thing with AI to teach myself how to make a thing with AI: [dadjokepostcards.com](https://www.dadjokepostcards.com). Pick a terrible joke, have it mailed on a postcard to someone who deserves it, and you donate to a good cause along the way.

This was inspired by wanting to keep some multichannel #dadjoke torture going even as my kids left for summer camp or college. That was a few years ago and I never got around to it, but recently, when I wanted to learn how to do AI-assisted coding, this seemed like a perfect project to cut my teeth on.

Some details about how it went and what I learned:

<!--more-->

I built it with [Claude](https://claude.ai), to see how far my rusty coding skills could take me building a real thing with an AI assist. Which is to say: I did none of the architecting, and almost none － at most 5% － of the coding. It took a single prompt and about five minutes to get a working prototype, and several hours after that to really get it going, but most of that time was spent setting up accounts at [Stripe](https://stripelcom) (for payment) and [Lob](https://lob.com) (for producing and mailing the postcards) and [Railway](https://railway.com) (hosting) and [OpenAI](https://developers.openai.com/api/docs/guides/moderation) (for their content moderation API). And I got picky and tweaked a lot about the design and wording of the cards. And had Claude fix many, many bugs. And had it research some business and policy and liability questions. And had it draft a letter of agreement for the nonprofit I decided to share most of the proceeds with.

In short, it turned out most of the work wasn't in being a hobby-level coder; it was in basically standing up a whole hobby-level business. (Fortunately, I already had a business construct for it at [The Key Jar](https://thekeyjar.com).) I learned a lot about working with nonprofits, responsibilities when using the USPS to transmit content, how selling postcards gets taxed, quirks of how Railway handles deployments ... all kinds of rabbit holes.

In all, I spent maybe 3-4 days' worth of time on it, over the course of a couple weeks.

I don't want to put too much on takeaways from a weekend project, but I think my labor distribution on this is pretty representative of what the future of a lot of service-level software production is going to be like. Tech- and AI-literate designers and product managers are in short supply and demand is already starting to explode for them.

Happy to talk more shop about how it went if anyone's curious.

The good cause: $2 of every card goes to the [Jazz Foundation of America](https://jazzfoundation.org). Why the Jazz Foundation? Because I love everything about them: bringing people of all backgrounds together over a shared American musical heritage at a divisive moment in our history, helping underpaid working and retired jazz and blues musicians in crisis, creating work for musicians, bringing more music to places like schools and nursing homes.

And aren't dadjokes a jazz-like art form? Ok, maybe that's a stretch.

<br/>
<br/>

![](/assets/images/dadjokepostcards-sample-sprite-7up.jpg)
*A typically bubbly dadjoke. Or did this one fall flat?*
