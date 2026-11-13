# ai-visibility-self-check: does AI recommend your business?

More and more people skip the search results and ask an AI assistant directly: "who's the best
pool cleaner near me?", "which dentist in Austin should I go to?". ChatGPT, Perplexity, Google's
AI answers and Copilot reply with two or three names.

Most local businesses are never one of those names. Usually not because they're worse, but
because the assistant can't find enough clear, consistent, independent information about them to
feel safe recommending them. The owner never finds out, because nobody gets a notification when
an AI leaves them out.

This repo is a way to find out by hand, in about 15 minutes, with a browser and free tools. No
software, no sign-up, no code.

## What's in here

```
CHECKLIST.md        10 checks, each with exact steps, what good and bad look like, and why it matters
SCORECARD.md        turns your answers into a rough score out of 100, split into 5 parts
sample-report/      a filled-in example for an invented pool cleaning company in Florida
```

The 10 checks:

1. Ask ChatGPT and Perplexity your customers' question, three times each
2. Sort every answer: recommended, mentioned, wrong business, or absent
3. Ask the assistants about you by name, and see which pages they use as sources
4. Compare your name, phone and address across Google, your site and your listings
5. Check that your website isn't telling AI crawlers to stay out (`robots.txt`, explained simply)
6. Check that both versions of your address load, and that Bing and Google know your pages
7. Read your homepage's first paragraph: does it say what you do and where?
8. Run Google's free Rich Results Test to see whether your facts are labelled for machines
9. Compare your reviews with the businesses the AI picked instead
10. Find out who else talks about you: lists, directories, local press

## How to use it

1. Open [CHECKLIST.md](CHECKLIST.md) and do the checks in order. Write your answers in the boxes.
   Check 1 takes the longest (about 5 minutes); most of the others take one or two.
2. Open [SCORECARD.md](SCORECARD.md) and turn your answers into points. It takes a few minutes and
   needs a calculator at most.
3. If you're not sure what a finished result looks like, read the
   [sample report](sample-report/README.md) first.

## What to do with the score

The scorecard ends with a short "what to do with it" list. In brief:

- **If your site blocks AI search crawlers, fix that first.** It's usually a single line.
- **Then make your name, phone and address identical everywhere.** It's free and every later
  improvement builds on it.
- **Then work on the part of the score that lost you the most points.** For most local businesses
  that's the off-site part: reviews, directories, and the "best of" lists the assistants read.
- **Re-run Checks 1 and 2 in 6 to 8 weeks**, the same way, and compare.

## What this is not

- **Not a guarantee.** Nobody can promise that a particular assistant will name you for a
  particular question. AI answers change from run to run and from week to week.
- **Not a precise measurement.** It's a hand-scored, rough reading. Use it to compare yourself
  with yourself over time, not with a number from some other tool.
- **Not a website audit.** A perfect website that nobody else mentions still doesn't get
  recommended. The heaviest part of the score is about what happens off your site, on purpose.

Every factual claim about how the AI crawlers work links to the company's own documentation in
[CHECKLIST.md](CHECKLIST.md) (Check 5), so you can check it yourself.

## License

MIT. Use it, change it, share it with your clients.

Built by [Milan Veljkovikj](https://github.com/milansolutionsai-ops).
