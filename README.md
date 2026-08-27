# Paste Bench

I got tired of doing the same annoying text stuff by hand over and over, so I made this. It's one HTML file, you open it in your browser, and that's it.

## Why I made this

Small annoyances like text copied from a PDF coming out all choppy, or needing to reformat a list five different ways, or making flashcards for a test. None of these are big enough that you'd go download an app for them, so you just deal with it every time instead.

## What's actually in it

**Dewrap**
This is the one I made first. Copy a paragraph out of a PDF and every line becomes its own broken line, and if a word got split across two lines it's got a random hyphen in the middle now. Dewrap fixes all of that: joins the lines back into normal paragraphs, fixes the hyphen-split words, straightens out the weird curly quotes PDFs sometimes use. It leaves actual paragraph breaks alone though, so it's not just mashing everything into one blob. You can also tell it to strip out HTML tags or pull out any URLs if you want.

**Listify**
Say you've got a column of stuff, names, cities, whatever, one per line. This spits it back out in like 8 different formats at once: comma separated, quoted, JSON, a SQL `IN (...)` clause, a markdown list, numbered, tab separated, pipe separated. Useful if you're bouncing between a spreadsheet and code a lot. It can sort and remove duplicates too. If your list actually looks like term-answer pairs, there's a button to send it straight to the Flashcards tab.

**Case & Slug**
Type something once, get it back in every casing style you'd ever need. camelCase, snake_case, kebab-case, UPPER CASE, Title Case, all of them, plus some goofy ones like alternating caps and just flat out reversed text.

**Word Count**
For when you need to hit a word count for an essay and don't want to open a whole word processor just to check. Shows word count, character count, how many sentences and paragraphs, your longest word, roughly how long it'll take to read, even a rough guess at what grade level it's written at. Set a target and it tells you how many words you've got left to go.

**Flashcards**
This one I'm actually pretty proud of. Type in term/definition pairs and hit start, and it turns into flip cards. But instead of just cycling through the same deck over and over, if you mark a card "still learning" it comes back around again later, and cards you get right just drop out. So you end up only really drilling the ones you don't know yet. Once you've gotten everything right at least once it shows you how long you took and exactly which cards gave you trouble and how many times.

**Group Picker**
For group projects or figuring out who goes first. Paste in names, shuffle them, pick one at random, pick a few winners, or split everyone into even groups. There's an option so it won't pick the same person twice until everyone's had a turn.

**Study Timer**
A pomodoro-style timer, focus time and breaks, switches automatically, does a longer break every 4 sessions. Has a little floating popup version too (only works in Chrome/Edge right now) that stays on screen even if you switch tabs, so you can keep an eye on it while you're doing something else. Also just added a small task list under it so you can jot down what you're actually working on that session.

## How to use it

Open `https://paste-bench.netlify.app`. That's genuinely it, there's no setup.

The only thing that needs a specific browser is the floating pop-out timer, since it uses an API that only Chrome and Edge support so far. Everything else works anywhere.

## What it's built with

Just HTML and fonts come from Google Fonts (IBM Plex Mono/Sans/Serif).

---

Made by XDabXking
