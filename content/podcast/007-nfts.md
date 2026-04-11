---
title: "007: NFTs"
date: "2021-06-04T03:33:26Z"
author: "Michael Edelheit"
categories:
  - "podcast"
tags:
  - "art"
  - "crypto"
  - "non-fungible"
  - "podcast"
slug: "007-nfts"
description: "How are NTFs currently being used in the real world? What goes into making an NFT? How do you make one from scratch? Find out on this week&#8217;s episode! Bonus Content: NFTs from scratch: Rinkeby test network Presentation link Episode Transcription &#8211; NFTs Liam&nbsp; 00:00 Hey everyone. Welcome to Episode 7 of Candid Crypto. Michael&#8230;"
---

How are NTFs currently being used in the real world? What goes into making an NFT? How do you make one from scratch? Find out on this week’s episode!

- [Google](https://podcasts.google.com/feed/aHR0cHM6Ly9jYW5kaWRjcnlwdG9wb2RjYXN0LmNvbS9wb2RjYXN0LnJzcw?sa=X&ved=0CAIQ9sEGahcKEwio_Jz57cnxAhUAAAAAHQAAAAAQBQ)
- [Spotify](https://open.spotify.com/show/6YXtKs9cvMU3XwvlqBegU7?si=X88I8tiSRpeGp2SWebny6Q&dl_branch=1)

Please leave a comment and let us know what you think about this episode. You can find Candid Crypto on all your favorite podcast platforms, so please like and subscribe to stay up to date on everything crypto!

In addition, every Candid Crypto episode is transcribed so you can easily understand everything that was discussed.

## Bonus Content: NFTs from scratch: Rinkeby test network

[Presentation link](https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbHQtSElzT3ZTY193d1ItVjktXzZHUXp0OFU3UXxBQ3Jtc0trMVNreUswRHNrRGFWc0V3VHIzeEV6VmU2d0RmZDhYLU1IYVhDaVZ5Zm1XZW80eThPM2NuM3RwYmJGaEhRcEdCZ0dHTEdiVnRheFBCdXhqSl9YamhVcVVQczVINm5LY3lmQWlLS3hMc2hUSGdrT0JaMA&q=https%3A%2F%2Ff002.backblazeb2.com%2Ffile%2Fcandid-crypto-public%2Fnft%2FOpenZeppelin%2BERC%2B721%2BToken%2BDeployment%2BTutorial.pdf)

**Episode Transcription – NFTs**

**Liam** 00:00

Hey everyone. Welcome to **Episode 7 of Candid Crypto**. Michael and I discuss NFTs. What problems do they solve? And how do you actually build one? For those who are interested in building an NFT, I made a technical tutorial whose link you can find on our website **@CandidCryptoPodcast.com**. Now onto the show.

There are also artists who use the Blockchain to get their fair share of commission from their streaming, from people streaming their music. I downloaded the app today called **Audius** and that’s supposedly a Blockchain powered music streaming platform. And I recognize some artists, there was like disclosure, dead mouse, other …

**Michael** 00:52

So what’s unique about this Blockchain music platform, then Spotify? Are they all NFTs essentially?

**Liam** 01:02

I don’t know. They didn’t seem to be that transparent. The big thing was that they were plugging their own token. And the more of their token you have, the higher your account ranks up. They didn’t make it immediately. obvious that, that was kind of the monetization of the platform. But yeah, these audio tokens are those I would keep an eye on for the next pump. This is not investment advice, by the way. Yeah, dude, I spent the past three days building the official candid crypto NFTs

**Michael** 01:47

I know it’s been a process.

**Liam** 01:48

Yeah, it has been a process, mostly because I didn’t want to pay Open Sea, or, you know, another service to create these things. I’m wanting to just see, okay. Like, I think I have enough kind of development and systems administration knowledge to maybe make one of these. Now, that being said, the platforms offer an easy way for you to do it. This was a lot

**Michael** 02:15

Much easier.

**Liam** 02:16

This was a little more technical. To make a long story short, I did that mostly because I wanted to uncover like, What the hell do you put on an NFT? Like, how do you actually build these things? And what kind of processes and tools are people using to make these? The ultimate takeaway was that the Blockchain serves a very specific purpose in this situation, it just lets you verify proof of ownership. By and large, most of the information about the NFT is stored somewhere else on the internet, not on the Blockchain. Which seems a little counterintuitive, but that’s how it works.

**Michael** 02:54

And I don’t want to get too much in the weeds. Because if people are really interested, though, they’ll check out your video as they should. But are you talking about finding a location to actually put it like the servers involved and hosting metadata,

**Liam** 03:12

Yeah, the metadata on the token that has to live somewhere else, you don’t put that into the Blockchain?

**Michael** 03:19

I mean, the working sessions that we had, and you walk in through the tutorial with me, that was- I had no experience using and it was cool to understand the metadata behind that NFTs.

**Liam** 03:31

Yeah. So what is an NFT? The definition we used in episode three. And what we talked about in our theorem episode, was that a **Non Fungible token** is something one of a kind, it is a token that exists quantity one, somewhere on a Blockchain. So it’s unique. There are not 10,000 of them minted at once. It’s just one and each token has unique properties.

**Michael** 04:01

And I mean, that really is the core of an NFT. I think it’s interesting. Looking at all the different use cases, it’s really not specific to one industry. NFTs can be used for so many reasons and can help so many people in different spaces you talked about, artists and musicians are now using NFTs to sell their artwork and really get a fair share of their earnings.

**Liam** 04:32

Yeah, a lot of use cases in the creative space for Non Fungible Tokens. You’re able to tokenize your artwork or at least a digital representation of your artwork. And you’re able to do that with music as well. And then fans can approve that they have their favorite artists NFTs, it’s certainly may seem a little alien to someone who hasn’t had experience with cryptocurrency but I have a feeling this is becoming a new trend. NFTs really came on the up and up in 2020. And while the crypto market as a whole kind of retracted these past few weeks. NFTs are still being bought and sold like crazy.

**Michael** 05:19

Yeah, I think the hype has settled a little bit, especially with just volatility in the cryptocurrency market in general. It’s definitely not as big of a bubble as some people said it was. I’m reading this off the internet. Auction House Christie’s soared the work of artists Beeples as an NFTs for $69 million. We spoke to that use case but I mean, that’s a ton.

**Liam** 05:46

That’s a ton of money. And there is certainly an argument to be made that these things are speculative, just like a lot of other crypto assets are which is true, you shouldn’t buy these things with the expectation that it will double your money next year. Rather the novelty and I suppose the cool factor, the digital identity, sort of paradigm to learn about each other. That is certainly taking off. It’s been validated by the fact that so much money is flowing into this space. And NFT as a search term became more popular than Cryptocurrency/Bitcoin at one point.

**Michael** 06:26

No way. I did not realize that I made I don’t know $69 million dollars. That’s a lot. That’s definitely an outlier. But I mean, there are hundreds of 1000s of dollars like people will pay like 10, 20, $100,000 for an NFT. These are like collectibles, not only just like art pieces, but just like random collectibles. I know that’s probably one of the second biggest use case is collectibles, if it’s sports collectibles, or even like **CryptoKitties**. Do you know what I’m talking about with CryptoKitties?

**Liam** 06:58

Yep.

**Michael** 06:59

Yeah, it’s like, I guess people find it valuable because it’s some of the first NFTs on the Ethereum network. And in 10 years, it will be like, Oh, this was… You know, even if it’s just a stupid little pixelated cat, like in 10 years, or like, what was just on the Blockchain such a long time ago. Isn’t that cool?

**Liam** 07:23

Yeah, exactly. When it’s a 10-year-old NFT. Maybe that’ll increase the cool factor?

**Michael** 07:27

I don’t know. I mean, $100,000. I don’t think it’s worth it. But I can see how some people are speculating, you know, this enormous amount of money for these NFTs.

**Liam** 07:39

So relating it back to our NFT. Our NFT is currently not live as of recording on June 2, Wednesday, on Friday, June the 4th, our NFT will be on the Ethereum main network, which means that you’ll be able to bid on it if you would like. Honestly, it’s a GIF. Like at the end of the day, this NFT is linked to a GIF that is hosted on the internet. That is all this is. By and large, NFTs are just digital representations of whatever media you can really drum up.

**Michael** 08:25

It can be an mp4, you know, an audio file, JPEG, whatever? I think that’s cool.

**Liam** 08:33

Yeah. And I’m sure as time goes on, we’ll figure out a lot more creative data to put into these NFTs, like tying them to real world assets in some sense, either. But we’re not there.

**Michael** 08:46

Well, we’re kind of getting there. I’ve heard about a few use cases where they’ll tie it to license or certifications like, I mean-

**Liam** 08:57

Whoa! interesting.

**Michael** 08:58

Yeah. Because it’s unique. And it’s way easier to validate that this individual has this license or certification if they just meant it as an NFT.

**Liam** 09:08

Right. Because then, ultimately, you’re just relying on the Blockchain to work not for the

**Michael** 09:14

Yeah. Oh, even like, this might be a little far out there but like a deed to your house. minted as an NFT.

**Liam** 09:24

Well, and ideally, that’s the direction we had in so as long as we could somehow figure out how to tie it to real world assets. When we manage to tie NFTs to real world assets, we will really see… Well, I should even say that, you know, because we haven’t thought about the things that NFTs can be used for tying them to real world assets seems like a cool thing to do. But in all likelihood, it’s going to be something else. It’s going to be probably related to data. There are just things that we’re really waiting for people to build at this point on top of this ecosystem.

**Michael** 09:58

Yeah, and I mean, the platforms We get way better. a) you can build your own, do your own website everything like we did on CandidCryptoPodcast.com. But there’s stuff like Open Seas, what are some other popular platforms.

**Liam** 10:18

So there’s also the one that I remember off the top of my head is called **Zora**. Z-O-R-A, **Rarible** and then **Minttable** is another one. Zara cargo. That’s what Open Sea is showing, okay, and also **Mintbase**, but I haven’t really used any of these tools myself. At the end of the day, all these tools are going to charge you extra money. So if you want to reclaim that portion that they take, then be sure to check out the supplemental video that I’m publishing on creating your own NFT and actually having it be live.

**Michael** 10:52

It’s pretty cool. We’re super excited to release our own NFT. Next is the Coin.

**Liam** 10:58

You know, on Candid Crypto, we don’t want to just talk the talk, we want to start building these things out. Even if they’re a little rudimentary, they definitely will allow people to maybe grasp the technology in a more relatable way when they get their hands on some Candid Crypto tokens-

**Michael** 11:19

Oh, yeah.

**Liam** 11:20

-Which I’m sure will be pretty generous with because they’re just tokens.

**Michael** 11:26

And Liam, it would be interesting. I mean, I watched you, or I’ve watched some of the working sessions that you’ve had to build this NFT. And it’s definitely not for everybody. It would be interesting for maybe me to mention NFT using the plug and play methods of the platforms, and we could do a little comparison of [crosstalk] processes.

**Liam** 11:51

I think that would be interesting. And then we could say, oh, like how are these? You know, technical underpinnings are different for how they kind of you deploy your NFT. Yeah, that would be…

**Michael** 12:05

I don’t think it’s that hard. I mean, it was hard at first to learn it. But now that you’ve learned it, and you talk people through the tutorial, it should be a lot easier.

**Liam** 12:15

Yeah, that’s tutorial was 15 minutes. I’d say I could do it front to back in about 15 or so. So we definitely sped up a bit, but it did take a lot of reading a lot of old forum posts.

**Michael** 12:32

Yeah, make your own and then sell it for millions of dollars. Good luck, everybody.

**Liam** 12:40Thanks for tuning to Candid Crypto. Remember **@CandidCryptoPodcast.com** reaches there. Take care everyone.
