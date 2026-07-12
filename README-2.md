# Things that actually helped me settle into Austin

A shared list of groups, events, volunteer shifts, and things to do — each one
with a note from a person who actually went, signed with their name.

It is not a directory. Directories rot and nobody trusts them. This is a list of
things that helped somebody, and it says who.

**Live site:** https://YOUR-USERNAME.github.io/violet-crown/

---

## Adding something

Three ways in, all of them one click from the site:

| I want to... | Use |
|---|---|
| Add a place/group/event that helped me | [➕ Add a resource](../../issues/new?template=add-resource.yml) |
| Say what one of these is *actually* like | [💬 Vouch for something](../../issues/new?template=add-note.yml) |
| Report a dead link or a folded org | [🔗 Something's wrong](../../issues/new?template=broken.yml) |

You don't need to know git. The forms are just forms.

**More than one note per entry is encouraged.** If you've been somewhere and your
experience was different from the note that's there — say so. Two honest opinions
beat one, and disagreement is more useful to a newcomer than consensus.

---

## What makes a good note

Not a description. A description is what the website already says. Write the part
a Google search can't tell you:

- **Who's in the room?** Age, seniority, vibe. Will a 24-year-old feel out of place?
- **Is anyone selling anything?** Recruiters trawling? A pitch disguised as a talk?
- **Can you show up alone?** Or do you need to know someone?
- **What do you do in the first five minutes?** The single most useful sentence you can write.

Two sentences is plenty. **It's fine to say something isn't worth it** — a list
that only praises is an advertisement.

---

## Setup (one time, ~10 minutes)

1. Create a public repo, upload `index.html`, `README.md`, and the `.github/` folder.
2. **Settings → Pages** → deploy from branch `main`, folder `/ (root)`. Save.
3. Open `index.html` and set two things at the top of the script:
   - `REPO` — your repo URL. **Every contribute button depends on this.**
   - `INTRO` — your own words about why you made it. Keep it first-person.
4. Check that **Settings → General → Issues** is enabled.

## Maintaining it

Editing the list means editing one array in `index.html`. Each entry:

```js
{id:"open-austin", bucket:"volunteer", cost:"free",
 name:"Open Austin",
 url:"https://www.open-austin.org/",
 when:"Monthly orientation call", where:"Remote + in person",
 what:"One factual sentence about what it is.",
 vouches:[
   {by:"Sam, moved from Chicago in 2025",
    note:"Went to the orientation call knowing nothing. Nobody cared that I'd never
          done civic tech. Ask which project needs a second pair of hands and just
          say yes to that one."}
 ],
 verified:"2026-07-11"}
```

When someone opens an issue, paste their words into `vouches` with their name,
close the issue, done. That's the whole workflow — thirty seconds a contribution.

**Every quarter:** click every link, bump the `verified` dates, close stale issues.
Half an hour, four times a year, is the entire cost of keeping this trustworthy.

If you ever stop maintaining it, **say so on the site.** A guide that admits it's
stale is still useful. One that quietly lies isn't.

---

Not sponsored. Not affiliated with anything listed. No tracking, no accounts,
no data collected — it's one HTML file.
