---
layout: post
title:  "dadjokepostcards.com, and its lessons for government digtial services"
date:   2026-09-16 00:00:00 -0400
# categories: dadjokes ai development
---

Hey, I made a thing with AI to teach myself how to make a thing with AI: [dadjokepostcards.com](https://www.dadjokepostcards.com). Pick a terrible joke, have it mailed on a postcard to someone who deserves it, and you donate to a good cause along the way.

This was inspired by wanting to keep some multichannel #dadjoke torture going even as my kids left for summer camp or college. That was a few years ago and I never got around to it, but recently, when I wanted to learn how to do AI-assisted coding, this seemed like a perfect project to cut my teeth on.

Some details about how it went and what I learned:

<!--more-->

**The work:** I built it with [Claude](https://claude.ai), to see how far my rusty coding skills could take me building a real thing with an AI assist. Which is to say: I did none of the architecting, and almost none － at most 5% － of the coding. It took a single prompt and about five minutes to get a working prototype, and several hours after that to really get it going, but most of that time was spent setting up accounts at [Stripe](https://stripelcom) (for payment) and [Lob](https://lob.com) (for producing and mailing the postcards) and [Railway](https://railway.com) (hosting) and [OpenAI](https://developers.openai.com/api/docs/guides/moderation) (for their content moderation API). And I got picky and tweaked a lot about the design and wording of the cards. And had Claude fix many, many bugs. And had it research some business and policy and liability questions. And had it draft a letter of agreement for the nonprofit I decided to share most of the proceeds with.

In short, it turned out most of the work wasn't in being a hobby-level coder; it was in basically standing up a whole hobby-level business. (Fortunately, I already had a business construct for it at [The Key Jar](https://thekeyjar.com).) I learned a lot about working with nonprofits, responsibilities when using the USPS to transmit content, how selling postcards gets taxed, quirks of how Railway handles deployments ... all kinds of rabbit holes. In all, I've spent maybe four person-days on this, spread out over the last couple months. That's less time than I would have spent on just the code in the pre-AI world.

**A couple takeaways:** A hobby-level project is hardly useful evidence for drawing generalizable lessons about the state of product design and development. But it was useful to experience first-hand what's obviously happening across the entire field: my labor distribution on this project, away from the code and onto the design and other non-technical tasks, is more or less representative of where service-level software production is (or is headed) now.

At [CDS](http://localhost:4000/2021/10/13/the-canadian-digital-service-chapter-1.html) we used to say "code is cheap," to encourage civil servants scarred by waterfall-driven development and absurdly expensive change orders not to think of software as something you have to very carefully plan, massively budget for, painstakingly build, and then never touch unless you absolutely must. Obviously code is cheaper than ever now, for any org ready and willing to take advantage of it.

And it's not just the code you and your team write yourselves that's cheaper now. Wiring up your code with other people's code is also easier and faster than ever. [dadjokepostcards.com](https://dadjokepostcards.com) is basically a thin wrapper that laces together a simple input form, the icanhazdadjoke API (I still chuckle every time I realize someone brought this into our world), an API that sends real mail for you (Lob), a payment API (Stripe), and a couple other components. Governments that give their departments and program offices a decent set of LEGOs to build with (what some have been calling [government as a platform](https://scispace.com/pdf/government-as-a-platform-y4jj5l8i5h.pdf) for a long time) are going to find it's easier than ever for those departments and programs to deliver services for their citizens more quickly, efficiently, consistently, securely, etc.

Governments, predictably, are all over the map. [The province of Alberta](https://nateglubish.substack.com/p/they-said-it-would-cost-54-million), of all places, is one of the first to use these developments to flip the script on how they interact with software vendors.)

The individuals who can power organizations to capitalize on this shift － tech-literate designers and product managers － were already in short supply pre-AI, and demand is exploding for them now. These are the AI-assisted versions of the "T-shaped" players we so prized at 18F and CDS: people who understand design and product, and who are also capable of [showing the thing](https://gds.blog.gov.uk/2014/06/03/principles-for-prototyping/). Someone who can teach those skills quickly and at scale is going to do very well.

Happy to talk more shop about all of this if anyone's curious.

**The good cause:** $2 of every card goes to the [Jazz Foundation of America](https://jazzfoundation.org). Why the Jazz Foundation? Because I love everything about them: bringing people of all backgrounds together over a shared American musical heritage at a divisive moment in our history, helping underpaid working and retired jazz and blues musicians in crisis, creating work for musicians, bringing more music to places like schools and nursing homes.

And aren't dadjokes a jazz-like art form? Ok, maybe that's a stretch.

<br/>

![](/assets/images/dadjokepostcards-sample-sprite-7up.jpg)
*A typically bubbly dadjoke. Or did this one fall flat?*
