---
title: Why Noisy Data?
published: 2025-08-20
draft: false
tags:
  - general
toc: false
coverImage:
  src: ./cover.jpg
  alt: A cartoon of a coder on a laptop, with a complex schema in the background.
description: "The first question I was asked: Why call it Noisy Data?  Simple, because all Data is Noisy!"
---
Why on earth call a personal blog Noisy Data?  Well, if there's one thing I've learned in nearly 25 years of wrangling data, it's that it's noisy, it's dirty, and it gets everywhere.  Its been described as the 'the new oil' and even 'the new plutonium'.   Data requires respect and careful handling.  Treat it well and it will provide insights and value.  Treat it badly and it has a tendency to leak and contaminate everything around it.

To kick things off, lets start with a short anecdote.  Back in the bygone days when I was a young intern, and the whole engineering department ran on less compute than the Raspberry Pis now discarded in my desk drawer, I was privileged to work with an amazing engineer called John.  John was a softly spoken gentleman who was a bridge to an even older age - that of punched card programming, big iron, and getting the results of your program several days after you submitted it to a computer a few hundred miles away.

John and I (well - I flatter myself I was helping!) were puzzling over some newly written code to compute the homogeneity of an MRI magnet.  For the non-physicists:  MRI magnets create a strong magnetic field, but the field must have a certain 'smoothness' or homogeneity in order to produce clear images.

The bug we were investigating was the code could only produce a couple of significant figures of accuracy; the rest was essentially noise.  Resorting to that most useful of debugging tools, the print statement, we noticed something:  All the numbers were identical bar some small variations at the 7th - 10th decimal places.

Every single freaking one of them.

The bug, for bug it was, was a failure to subtract the big background field of the magnet from the small measurements of field variation we were trying to compute.  In John's immortal words at the time:

> Like trying to subtract two elephants from each other in order to weigh the fleas.

I hadn't paid attention to the data we were inputting.  Turns out there was a difference between differential and absolute measurement that I'd missed completely.  Classic Garbage In, Garbage Out.  

So that's the lesson, and why I've started to write this blog:  Treat the data right, respect how it's collected, what it represents, how it should be handled and modelled, and you will build successful products, gain insights and new knowledge.  Treat it badly, and all you'll have is a noisy, hot mess.

Happy reading!
