---
title: "Collaborative Risk Register"
date: 2026-03-17
---

In the [last thing I wrote](prototypes-with-claude.md), I started working on a prototype with the primary goal of seeing how quickly I could spin up a decent one with Claude Code.
[DARPI](https://github.com/konnerhorton/darpi) is the result. The name (an acronym for "Don't Accept Risk, Price It") still needs some work, it sounds a bit cheesier than the product should be, but I'm pretty pleased with the process I used and how good the prototype is after about 2 working days of effort.

To get to this point, I started with an initial prompt of an idea, had Claude read it, then from there went into planning mode and develop a `PRODUCT_VISION.md` document and a `PROTOTYPE_SPEC.md` that Claude used to build the tool.
You can see more of the details of those two documents and the process in the [repo](https://github.com/konnerhorton/darpi).

The idea behind this risk register is that when we use Excel we loose so much of the metadata and process documentation that is useful in these contexts.
Some features I was going for include:
- One-to-many relationships between risks and mitigations (because one mitigations might benefit many risks)
- Run analysis on the fly (though sometimes you want to keep the results hidden from participants from the end, to reduce biases in subsequent assessments)
- Ability to suggest then accept / reject scoring values, with a comment log to track the discussion.
- Snapshots that allow the facilitator, at the end of a workshop or session, to save the current state to review in the future.
- Have the interface optimized for a keyboard-driven workshop in a virtual meeting (hopefully the user does not have to touch their mouse, so data input does not lag discussion, though perhaps this could be eliminated all together with a AI model doing that work).

While it was a good way to get to understand Claude Code a little better, I'm not so sure its a product worth pursuing, at least on its own.
The stickiness of Excel remains, and sometimes the chaos that it can bring is a feature, not a bug.
Like a lot of process documentation in the construction industry, some version of [Goodhart's Law](https://en.wikipedia.org/wiki/Goodhart's_law) applies.
The generation of documents becomes the goal as opposed to solutions that those documents are supposed to initiate.
So, the back and forth of an Excel file, with its resultant uncertainty in versioning, generates more documents and discussion, satisfying bureaucratic goals but not necessarily facilitating project execution.

I think, however, it could be useful as part of a larger platform, where users are already collaborating on other work and this would be just another tool that they have.