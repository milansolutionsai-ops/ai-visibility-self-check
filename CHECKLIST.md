# The checklist: 10 checks, about 15 minutes

You need a browser, the free versions of ChatGPT and Perplexity, and your website address.
No accounts to create beyond those, no software to install.

Work through the checks in order. Write down what you find as you go (the boxes at the end of
each check), then carry your answers into [SCORECARD.md](SCORECARD.md).

Two words used throughout:

- **AI assistant**: ChatGPT, Perplexity, Google's AI answers, Copilot, Claude and the like.
- **Listing**: any page about your business that you don't own: your Google Business Profile,
  Yelp, Facebook, BBB, Apple Maps, Bing Places, trade directories.

---

## Check 1. Ask the AI the question your customers ask (5 minutes)

This is the one that matters most, so it goes first.

**What to do**

1. Write down the question a new customer would type. Use their words, not yours:
   `best [service] in [city]`. For example: `best pool cleaning service in Tampa`.
   Write a second one in problem form: `who should I hire to [fix the problem] in [city]`.
2. Open ChatGPT. Start a **temporary chat** (top of the screen) so your own chat history
   doesn't steer the answer. Paste the first question. Read the answer.
3. Open a **new** temporary chat and ask the same question again. Do it a third time.
4. Do the same in Perplexity: three new threads, same question.
5. If you have time, repeat with the second question.

**Why three times:** AI assistants don't give the same answer twice. One run that leaves you
out proves very little. Three runs show you a pattern.

**What good looks like:** you are named as a recommendation in at least 2 of the 3 runs on each
assistant.

**What bad looks like:** you appear in none of the 6 runs, while the same 2 or 3 competitors
keep coming back.

**Why it matters:** this is literally what a customer sees. Everything else on this list is an
explanation for the result you get here.

Write down for each run: which businesses were named, and where you were (see Check 2).
Also write down the names that keep appearing. You'll use them in Checks 9 and 10.

---

## Check 2. Mentioned is not recommended (2 minutes)

Don't count a run as a win just because your name shows up somewhere in the text. Read the
sentence your name is in, and put each of the 6 runs from Check 1 into exactly one box:

| Box | What it looks like |
|---|---|
| **Recommended** | You are given as an answer to the question. "Top options include ... [you]." |
| **Mentioned** | Your name is there, but in passing. "Other companies in the area include ...", or as the one being compared against. |
| **Wrong business** | Your name appears, but the sentence describes someone else: a different company with a similar name, another town, a service you don't offer. |
| **Absent** | You're not there. |

**What good looks like:** mostly Recommended.

**What bad looks like:** any Wrong business. This is worse than Absent. The assistant is
confidently telling customers something false about you, and they have no way to know.

**Why it matters:** "our name came up" is the easiest result to misread. A tool that just
searches the answer for your name will count a passing mention, or even a different business
with your name, as a success. Read the sentence.

| Run | ChatGPT | Perplexity |
|---|---|---|
| 1 | | |
| 2 | | |
| 3 | | |

---

## Check 3. Ask the AI about you by name (2 minutes)

**What to do**

1. In a new ChatGPT temporary chat, ask: `What do you know about [your business name] in [city]?`
2. Ask the same in Perplexity.
3. Compare the answer with the truth: services, area, phone, how long you've been around.
4. Look at the sources each assistant shows (links, footnotes, the "Sources" panel). Write down
   which pages it used. Is your own website one of them, or only Facebook, LinkedIn, Yelp,
   a directory?

**What good looks like:** the description is correct, and your website is among the sources.

**What bad looks like:** wrong details, an old address or phone, a mix of you and another
business, or "I don't have information about that business." Also a warning sign: the
assistant describes you only from a social profile or directory, never your own site.

**Why it matters:** an assistant repeats what it can find and cross-check. If the clearest
description of you lives on someone else's page, that page decides how you're described,
and your site isn't treated as the main source about you.

---

## Check 4. Same name, same phone, same address, everywhere (3 minutes)

**What to do**

1. Search Google for your business name. Open your Google Business Profile.
2. Open your website's contact page.
3. Search for your name on Yelp, Facebook, BBB, Apple Maps (or Bing Places) and the one or two
   directories that matter in your trade.
4. Fill in the table. Copy exactly what each page says, including "LLC", "& Sons", suite
   numbers, area codes.
5. While you're on each site, check whether **two** profiles exist for you (an old one from a
   previous address, a duplicate someone created).

| Where | Name as written | Phone | Address |
|---|---|---|---|
| Google Business Profile | | | |
| Your website | | | |
| Yelp | | | |
| Facebook | | | |
| BBB / trade directory | | | |

**What good looks like:** every row is identical, and there's one profile per site.

**What bad looks like:** two phone numbers in circulation, two addresses (an old one and a new
one, or a home address and a business address), name variants, or duplicate profiles.

**Why it matters:** an AI assistant is trying to work out whether all these pages describe the
same business. When the details disagree, it can't be sure, so instead of one business with a
lot of evidence behind it, it sees two or three businesses with a little evidence each. Fixing
this is usually free and is often the biggest single improvement a local business can make.
Decide which version is correct before you change anything, then change everything to match it.

---

## Check 5. Does your website let AI crawlers in? (1 minute)

AI assistants send automated visitors ("crawlers" or "bots") to read websites. Every website can
leave a note at the front door saying which bots may come in. That note is a plain text file
called `robots.txt`.

**What to do**

1. In your browser, go to `https://yourwebsite.com/robots.txt` (your address, then `/robots.txt`).
2. Look at what loads.

**How to read it.** The file is made of short groups like this:

```
User-agent: *
Disallow: /admin
```

`User-agent` names the bot the rule is for (`*` means every bot). `Disallow` names what that bot
may not read. Only one line is a real problem: `Disallow: /` with nothing after the slash, under
a bot that powers AI search. That means "this whole website is off limits."

| Bot name in the file | Who it belongs to | If it has `Disallow: /` |
|---|---|---|
| `*` | every bot | Problem. Nothing can read your site. |
| `OAI-SearchBot` | OpenAI, for ChatGPT search | Problem. OpenAI says opted-out sites are not shown in ChatGPT search answers. |
| `PerplexityBot` | Perplexity | Problem for Perplexity answers. |
| `Claude-SearchBot` | Anthropic, for Claude's search | Problem for Claude's search answers. |
| `Bingbot` | Microsoft Bing, which Copilot answers from | Problem. |
| `GPTBot`, `Google-Extended`, `CCBot` | Collect data for training AI models | Not a visibility problem. Blocking these is a choice about training, not about being found. Google says `Google-Extended` does not affect inclusion in Google Search. |

**What good looks like:** no `Disallow: /` under `*` or under any search bot above. A page that
says "not found", or an empty file, is also fine: it means nothing is blocked.

**What bad looks like:** `Disallow: /` under `User-agent: *` or under a search bot. These are
often left over from when the site was being built.

**Rules that are fine and look scary:** `Disallow: /wp-admin/`, `Disallow: /cart`,
`Disallow: /admin`. They block one private corner, not the site.

**One thing this check can't see:** some hosting and security services block bots before they
ever reach `robots.txt`. If everything above looks fine but you still never appear anywhere, ask
whoever runs your website: "Does our bot protection or firewall block AI crawlers like
OAI-SearchBot or PerplexityBot?"

Sources for the bot names: [OpenAI](https://platform.openai.com/docs/bots) ·
[Perplexity](https://docs.perplexity.ai/guides/bots) ·
[Anthropic](https://support.anthropic.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler) ·
[Google](https://developers.google.com/search/docs/crawling-indexing/google-common-crawlers) ·
[how robots.txt works](https://developers.google.com/search/docs/crawling-indexing/robots/intro)

---

## Check 6. Can the site be reached, and do search engines know your pages? (1 minute)

**What to do**

1. Type `https://yourwebsite.com` and then `https://www.yourwebsite.com` into the address bar.
   Both should open your site with a padlock and no security warning.
2. Go to [bing.com](https://www.bing.com) and search `site:yourwebsite.com`. Do the same on
   Google. Count roughly how many of your pages come up.

**What good looks like:** both addresses open cleanly. Bing and Google both list your main pages
(home, each service, contact).

**What bad looks like:** one of the two addresses shows "Your connection is not private". Or one
search engine lists only your homepage, or nothing at all.

**Why it matters:** a page that throws a security error, or that a search engine has never
seen, can't be used as a source. Microsoft Copilot answers from Bing, and owners rarely check
Bing because they only look at Google. If Bing shows little or nothing, submitting your site at
[Bing Webmaster Tools](https://www.bing.com/webmasters) is free.

---

## Check 7. Does your first paragraph say what you do and where? (1 minute)

**What to do**

1. Open your homepage. Read only the first two or three sentences of real text (skip the menu).
2. Ask: could a stranger answer these from those sentences alone?
   - What do you do?
   - Where do you do it?
   - Who is it for?

**What good looks like:** "[Your name] cleans and repairs home pools in Tampa and St. Petersburg,
weekly or one-off." Plain, specific, one breath.

**What bad looks like:** a slogan ("Your oasis awaits"), a welcome message, or a story about how
the business started, with the actual service three scrolls down.

**Why it matters:** AI assistants quote short passages, not whole pages. A passage that answers
the question directly can be lifted into an answer. A passage that only sets a mood can't. Do the
same test on each service page: the first sentence should say what that service is and where you
offer it.

While you're here, note two more things for the scorecard: do you have a separate page for each
main service, and is there a questions-and-answers section (price range, area covered, how soon
you can start)?

---

## Check 8. Are your facts labelled for machines? (2 minutes)

A person reading your site knows that `(555) 010-0000` is your phone number. A machine only sees
digits. Websites can carry hidden labels (called **structured data** or **schema**) that say
"this is a business, this is its name, this is its phone, these are its hours." Without the
labels, the machine is guessing. With them, it knows. If you sell many products, courses or
services, each one needs its label too, or the machine can't tell them apart from the rest of
the page.

**What to do**

1. Go to Google's free [Rich Results Test](https://search.google.com/test/rich-results).
2. Paste your homepage address and run it.
3. Look at the list of detected items. You want to see a business item (it may be called
   Local business, Organization, or something more specific to your trade).
4. Click into it. Check the name, address and phone it shows against your table from Check 4.
5. For the full picture, paste the same address into the
   [Schema Markup Validator](https://validator.schema.org/). It lists every label on the page,
   including ones Google doesn't show, such as opening hours and links to your other profiles.

**What good looks like:** a business item is detected, and its name, address and phone match
your Google Business Profile exactly. Hours and links to your social and directory profiles are
there too.

**What bad looks like:** "No items detected". Or a business item that carries an old phone or
address, which spreads the Check 4 problem into the machine-readable layer as well.

**Why it matters:** labels don't make an assistant recommend you on their own. What they do is
remove doubt about who you are, which is the thing Check 4 is about. Use these two tools rather
than viewing the page source yourself: website builders often add labels with code that only
runs in a browser, and these tools run the page the way a browser does.

---

## Check 9. Reviews: yours against the businesses AI picks (1 minute)

**What to do**

1. On your Google Business Profile, note your star rating, your number of reviews, and the date
   of the newest one.
2. Do the same for the two businesses that appeared most in Check 1.
3. Check whether you reply to reviews.

**What good looks like:** your review count is in the same range as theirs, you received a review
in the last month, and reviews get replies.

**What bad looks like:** a great rating on a handful of reviews, while the business AI keeps
naming has ten times as many. Or reviews spread across several platforms and duplicate profiles
(see Check 4), so no single profile looks established.

**Why it matters:** reviews are other people saying you're good, on a site you don't control.
That kind of evidence carries more weight than anything you say about yourself.

---

## Check 10. Who else talks about you? (2 minutes)

**What to do**

1. Search Google for the question from Check 1, word for word. Open the "best of" articles and
   directory pages on the first page of results. Are you on any of them?
2. Look at the sources Perplexity showed you in Check 1. Open two or three. Are you on them?
3. Search for your name while hiding your own site: `"Your Business Name" -site:yourwebsite.com`.
   Count the pages that talk about you and aren't yours.
4. Take your two proudest claims (years in business, a certification, an award, "largest in the
   county"). Search for each. Does anyone besides you say it?

**What good looks like:** you're on at least one of the lists the assistants and Google keep
using, a local news piece or association page mentions you, and your main claims appear on
someone else's site too.

**What bad looks like:** the only pages about you are your own site and your own social
profiles. Your claims exist only on your homepage.

**Why it matters:** this is the heaviest part of the score, on purpose. A business praising itself
is a weak signal; an independent page saying the same thing is a strong one. The "best of" lists
from step 1 are often exactly where AI answers come from. Getting onto them (by asking the
publisher, joining the directory, or being worth writing about) is slow work, and it's usually the
work that moves Check 1.

---

Done. Take your notes to [SCORECARD.md](SCORECARD.md).
