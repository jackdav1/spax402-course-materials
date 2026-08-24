# SPAX 402 — Course Materials

Predictive Analytics with Athletics Data · University of Delaware · Fall 2026

This repository holds the shared course content: lecture decks, weekly quiz banks, and any
shared data. You pull from it; you never commit to it.

## Setup

Clone it **next to** your own course repo, not inside it:

```
spax402-course-materials/   <- you pull
spax402-<your-name>/        <- you commit
```

Then run `git pull` here at the start of each week. New weeks appear as they are released.

`/quiz-me` in your own repo reads the week's question bank from this repository. If it can't
find this clone, it will tell you so rather than making questions up. If you keep this repo
somewhere other than next to your own, set the `SPAX402_MATERIALS` environment variable to its
path.

## Layout

```
decks/                 lecture decks, one per week
weeks/weekNN/          quiz bank and any shared files for that week
```
