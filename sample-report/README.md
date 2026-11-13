# Sample report: a pool cleaning company in Central Florida

> **This business is invented.** The name, town, phone numbers, addresses, review counts and
> competitors below are made up. The *pattern* is real: it follows an actual audit of a local
> service business, with every detail changed so it can't be traced back. Phone numbers use the
> 555-01xx range, which is reserved for fiction.

**Business:** Lanai Pool Care (invented), weekly pool cleaning and green-pool recovery
**Area:** Cedar Lake (invented town) and nearby towns, Central Florida
**Customers ask in:** English
**Checked by hand, using:** [CHECKLIST.md](../CHECKLIST.md) and [SCORECARD.md](../SCORECARD.md)

---

## The short version

**Score: 23 out of 100.** When a homeowner asks ChatGPT or Perplexity for the best pool cleaning
service in Cedar Lake, the town where this business is based, it doesn't come up. In 6 runs it
was named once, as an also-ran, and never recommended.

The business itself is good: 4.9 stars on Google, a same-week "clear water or we come back"
guarantee. The problem isn't quality. The problem is that online it looks like **three different
small companies** instead of one solid one:

- two phone numbers in circulation,
- two addresses (an old one in another town, and the current one),
- three versions of the name ("Lanai Pool Care", "Lanai Pool Care LLC", "Lanai Pool Service"),
- two BBB profiles and two profiles on a home-services directory.

An AI assistant trying to decide whether it can trust this business finds three thin piles of
evidence instead of one thick one, and recommends the competitor whose details all agree.

---

## Score

| Part | Points (of 10) | Share | Weighted | Main finding |
|---|---|---|---|---|
| 1. Technical access | 4 | 15 | 6.0 | `robots.txt` is empty, so nothing is blocked. But `www.` shows a security warning, and Bing and Google only know the homepage. |
| 2. Structured data | 4 | 10 | 4.0 | Labels are there, added by the website builder. They carry the **old** phone and the **old** town. |
| 3. Content | 2 | 20 | 4.0 | The homepage opens with a slogan. One page for everything, no questions-and-answers. |
| 4. Entity and off-site | 2 | 35 | 7.0 | Details disagree across listings. Duplicate profiles. On none of the "best of" lists. |
| 5. Live citation | 1 | 20 | 2.0 | 0 recommended, 1 mentioned, 5 absent. |
| **Total** | | | **23** | |

Blocked front door rule: does not apply.

---

## Check by check

### Check 1 and 2: what the assistants said

Question: `best pool cleaning service in Cedar Lake FL`, 3 fresh temporary chats in ChatGPT,
3 new threads in Perplexity.

| Run | ChatGPT | Perplexity |
|---|---|---|
| 1 | Absent | Absent |
| 2 | Absent | **Mentioned** ("other local options include...") |
| 3 | Absent | Absent |

Who got recommended instead:

| Competitor | Times recommended (of 6) | What they have |
|---|---|---|
| Competitor A | 6 | About 520 Google reviews, one name and one phone everywhere, on every "best of" list checked |
| Competitor B | 4 | A national franchise, appears on trade-association rankings |
| Competitor C | 3 | Strong Yelp profile with photos and prices |

Second question (`who should I hire to clean my pool in Cedar Lake`): same three competitors,
Lanai absent in all 6.

### Check 3: asked about by name

- **Perplexity** found the business and described it correctly, but gave the **old** address in
  the other town. Sources it showed: the old BBB profile and a directory listing. Not the website.
- **ChatGPT** blended the two directory profiles and listed both phone numbers, as if they were
  two branches.

The business's own website wasn't among the sources in either answer.

### Check 4: name, phone, address

| Where | Name as written | Phone | Address |
|---|---|---|---|
| Google Business Profile | Lanai Pool Care | (555) 010-0142 | 18 Heron Way, Cedar Lake |
| Website | Lanai Pool Care LLC | (555) 010-0142 | Cedar Lake (no street) |
| BBB profile 1 | Lanai Pool Care LLC | (555) 010-0142 | 18 Heron Way, Cedar Lake |
| BBB profile 2 | Lanai Pool Service | (555) 010-0187 | 902 Mill Creek Rd, Oak Ridge |
| Directory profile 1 | Lanai Pool Care | (555) 010-0142 | Cedar Lake |
| Directory profile 2 | Lanai Pool Service | (555) 010-0187 | Oak Ridge |
| Facebook | Lanai Pool Care | (555) 010-0187 | not listed |

The second phone and the Oak Ridge address belong to an earlier, now inactive version of the
business. Nobody closed those profiles.

### Check 5: robots.txt

Empty file. That means every bot is allowed. Nothing to fix here.

### Check 6: reachable and known

- `https://lanaipoolcare.example` opens fine. `https://www.lanaipoolcare.example` shows
  "Your connection is not private". Anyone (or any bot) typing the `www` version hits a warning.
- `site:` search: Google lists the homepage and one blog post. Bing lists the homepage only.

### Check 7: first paragraph

Current opener: *"Relax, we've got your backyard covered."* It says nothing about pools, place or
customer. The service, the area and the guarantee are all further down the page, in separate blocks.

### Check 8: labels

The Rich Results Test found a business item. So did the Schema Markup Validator. But the phone in
it is the old (555) 010-0187 and the town is Oak Ridge. No opening hours, no links to the other
profiles.

**Worth knowing:** looking at the raw page code, there appeared to be no labels at all. The
website builder adds them with code that only runs in a browser. The two free tools run the page
like a browser does, which is why the checklist uses them. A quick look at the source would have
reported "no labels" and sent the owner to fix something that existed.

### Check 9: reviews

| | Rating | Reviews | Newest review |
|---|---|---|---|
| Lanai Pool Care | 4.9 | 38 | 2 weeks ago |
| Competitor A | 4.7 | about 520 | 3 days ago |

The rating is better than the leader's. The volume is a fraction of it, and another 11 reviews
sit on the duplicate profiles where they help nobody.

### Check 10: who else talks about them

- First page of Google for the money question: four "best pool service" list articles and two
  directories. Lanai is on none of them. Competitor A is on all six.
- `"Lanai Pool Care" -site:lanaipoolcare.example`: the listings above and nothing else. No local
  news, no association page.
- The "clear water or we come back" guarantee appears only on the business's own homepage.

---

## What to do, in order

### This week (free, in the owner's control)

1. **Pick one name, one phone, one address.** The owner decides which is correct. Then change
   every listing in the Check 4 table to match, and close or merge the duplicate BBB and directory
   profiles. Biggest single fix on this list.
2. **Fix the `www` warning.** Either make `www.` redirect to the main address, or add a
   certificate that covers it. Usually a setting in the website builder or the domain host.
3. **Update the labels** to the chosen name, phone and full street address, and add opening hours
   and links to the Google, Facebook, BBB and directory profiles.
4. **Rewrite the homepage opener.** Something like: *"Lanai Pool Care cleans and repairs home
   pools in Cedar Lake and nearby towns, weekly or one-off. If the water isn't clear after a visit,
   we come back the same week."*

### Next 30 days

5. **Submit the site in Bing Webmaster Tools**, and in Google Search Console if that isn't done yet.
6. **Add a page per service** (weekly cleaning, green-pool recovery, equipment repair) and one per
   main town served, each opening with a plain sentence about what and where.
7. **Add a questions-and-answers section** with the questions customers actually ask on the phone:
   price range, area covered, how soon the first visit can be, what happens if the water still isn't clear.
8. **Ask for a Google review after every visit**, and reply to every review.

### Next 90 days (slower, and the part that moves the result)

9. **Get onto the lists.** Contact the publishers of the four "best pool service" articles and the
   two directories from Check 10. These are the pages the assistants are reading.
10. **Get the guarantee said somewhere else.** A local news piece, a neighbourhood group, a
    trade-association profile: anywhere independent that repeats what the homepage claims.
11. **Re-run Checks 1 and 2** in 6 to 8 weeks with the same two questions, the same way.

### What the fixes can and can't do

If every fix in "this week" and "next 30 days" were done, the scorecard would read about 64 out
of 100 before any change in what the assistants say. That's the ceiling of work on your own
website and listings. The rest of the score, and the actual recommendations, come from items 9
to 11: other people saying it. That part takes months, and no one can promise a date.

---

## How this sample was made

The findings come from a real audit of a real local business. For this sample, the name, town,
streets, phone numbers, review counts, star ratings, competitor names and the wording of every
AI answer were invented or changed. The proportions and the order of the problems were kept,
because that's the useful part: a good business, split into three on the internet, losing to a
competitor whose details agree everywhere.
