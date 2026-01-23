---
title: "WASM Web Apps"
date: 2026-01-23
---

Last year I learned about [marimo notebooks](https://marimo.io/) (as a substitute for [Jupyter notebooks](https://jupyter.org/)) and have since been trying to play around with them.
One nice feature is that you can very quickly deploy a notebook as a [WASM web app](https://en.wikipedia.org/wiki/WebAssembly).
These are static sites that can function as web apps that run entirely in the browser (client-side).

Why is that interesting?

There are times when I have built, for myself, utilities to perform some simple data-related tasks or calculations that Excel is poorly suited for (or I just didn't want to write in Excel because it's less fun).
The problem with these is their difficulty in sharing.
Many corporate IT environments frown upon excessive, or any, opensource software use.
And, generally, my colleages don't want to learn how to install Python and set up an environment just so they can save some manual work.

So, I can write some Python logic/workflow in a marimo notebook, add some input/output user interfaces and once it is dialed in, publish it to Github for free.
Then anyone with the url can use the app.
And like with any python-related work, [claude code](https://code.claude.com/docs/en/overview) can help out a lot.
Meaning I can get it running a lot faster, and do less fiddling with tests and user interfaces.

My first go at this for general use is to help with interval joins between a table with lithologies / geologic description and can be found here: [geology-joins](https://konnerhorton.github.io/geology-joins/)

[Streamlit](https://streamlit.io/) is another option for something similar, though its a proper server-side web app that requires a few more steps (but not many) to go from scripts to app.
