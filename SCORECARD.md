# The scorecard

Turn your notes from [CHECKLIST.md](CHECKLIST.md) into a rough score out of 100.

The score is split into five parts. Each part gets a few points from 0 to 10, then counts for a
share of the total. The shares are not equal on purpose: what other people say about you counts
for more than anything on your own website.

| Part | Share of total | Checks | The question it answers |
|---|---|---|---|
| 1. Technical access | 15 | 5, 6 | Can AI tools reach and read your site at all? |
| 2. Structured data | 10 | 8 | Are your facts labelled so a machine knows what they are? |
| 3. Content | 20 | 7 | Does your site answer customer questions in quotable sentences? |
| 4. Entity and off-site | 35 | 3, 4, 9, 10 | Is it clear who you are, and do others back it up? |
| 5. Live citation | 20 | 1, 2 | Do AI assistants actually name you today? |

For every line below: full points if the answer is clearly yes, **half** if it's partly true,
zero if no. Don't round up. Nobody else sees this sheet.

---

## Part 1. Technical access (share: 15)

| | Line | Points | Yours |
|---|---|---|---|
| T1 | `robots.txt` has no `Disallow: /` under `*`, `OAI-SearchBot`, `PerplexityBot`, `Claude-SearchBot` or `Bingbot` (Check 5) | 4 | |
| T2 | Both `yoursite.com` and `www.yoursite.com` open with a padlock, no warning (Check 6) | 3 | |
| T3 | Bing **and** Google list your main pages, not just the homepage (Check 6) | 3 | |
| | **Part 1 total (out of 10)** | | |

**Blocked front door rule:** if T1 scored 0 because a whole-site `Disallow: /` covers a search
bot, your final score can't go above **35**, however well the rest goes. Nothing else pays off
until that's fixed. (A block on `GPTBot` or `Google-Extended` alone doesn't trigger this rule.
Those are training opt-outs, see Check 5.)

## Part 2. Structured data (share: 10)

| | Line | Points | Yours |
|---|---|---|---|
| S1 | The Rich Results Test finds a business item on your homepage (Check 8) | 4 | |
| S2 | That item's name, address and phone match your Google Business Profile exactly | 3 | |
| S3 | The Schema Markup Validator also shows your opening hours and links to your other profiles | 3 | |
| | **Part 2 total (out of 10)** | | |

## Part 3. Content (share: 20)

| | Line | Points | Yours |
|---|---|---|---|
| C1 | The first two or three sentences of your homepage say what you do, where, and for whom (Check 7) | 4 | |
| C2 | Each main service (or each main area you serve) has its own page that opens the same way | 3 | |
| C3 | There's a questions-and-answers section with plain answers to real customer questions: price range, area, how soon you can start | 3 | |
| | **Part 3 total (out of 10)** | | |

## Part 4. Entity and off-site (share: 35)

| | Line | Points | Yours |
|---|---|---|---|
| E1 | Name, phone and address are identical on your site, Google and every listing you checked, with no duplicate profiles (Check 4) | 3 | |
| E2 | Asked about you by name, both assistants describe you correctly, and neither confuses you with another business (Check 3) | 2 | |
| E3 | Your review count is in the same range as the businesses AI named, and you had a review in the last month (Check 9) | 2 | |
| E4 | You're on at least one "best of" list or directory page that Google or the assistants keep showing, and your main claims appear on someone else's site (Check 10) | 3 | |
| | **Part 4 total (out of 10)** | | |

## Part 5. Live citation (share: 20)

From Check 2, count your 6 runs (3 ChatGPT, 3 Perplexity):

- Recommended runs: ______
- Mentioned runs: ______
- Wrong business runs: ______

**Part 5 total** = (2 × Recommended) + (1 × Mentioned), capped at 10.

If **2 or more** runs were Wrong business, Part 5 is **0** no matter what else happened. An
assistant describing someone else under your name is worse than silence.

---

## Add it up

| Part | Your points (out of 10) | × share ÷ 10 | Weighted |
|---|---|---|---|
| 1. Technical access | | × 15 ÷ 10 | |
| 2. Structured data | | × 10 ÷ 10 | |
| 3. Content | | × 20 ÷ 10 | |
| 4. Entity and off-site | | × 35 ÷ 10 | |
| 5. Live citation | | × 20 ÷ 10 | |
| **Total (out of 100)** | | | |

Example: Part 4 at 4 out of 10 is worth 4 × 35 ÷ 10 = 14 points.

Apply the blocked front door rule from Part 1 last.

## What the number means

| Score | Reading |
|---|---|
| 0 to 39 | AI assistants can't find enough about you to name you. Customers asking them never hear of you. |
| 40 to 69 | You exist to the machines, but the evidence is thin or split, so someone else gets named first. |
| 70 to 100 | The foundations are in place. What's left is mostly earning more independent mentions over time. |

This is a hand-scored, rough reading. It is not comparable to any tool's score, and two people
scoring the same business will land a few points apart. Use it to compare **yourself with
yourself** a couple of months from now.

## What to do with it

1. **If the blocked front door rule applied, fix that first.** It's usually one line in one file,
   and nothing else matters until it's done.
2. **Then fix Check 4 (name, phone, address).** It's free, it's in your control, and every review
   and mention you earn afterwards lands on one business instead of being split.
3. **Then look at which part lost you the most weighted points**, and start there. For most local
   businesses this is Part 4: the site is fine, and nobody else is talking about them.
4. **Don't spend weeks on Parts 1 to 3 if they're already decent.** A tidy website that nobody
   else mentions still doesn't get named. Past a basic level, the next point comes from outside
   your site.
5. **Re-run Check 1 and Check 2 in 6 to 8 weeks**, with the same questions, the same way. Changes
   to listings and reviews take weeks to show up in AI answers, and some take months. Compare the
   Recommended count, not your feelings about one answer.

What this can't promise: no checklist, tool or agency can guarantee that a specific assistant
names you for a specific question. What you control is how easy you are to find, check and
trust. The score measures that.
