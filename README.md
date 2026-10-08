# Portfolio details

Three small details that make a portfolio easier to read in the 30 seconds most people give it. **[See all three live](https://miguelclavel.github.io/portfolio-details/)** · one file, no libraries.

## 1. A list that remembers what you opened

Good case study pages just sit there. Great ones remember if you already looked.

On my site, once you open a case study and come back to the list, a small dot and the word "Viewed" show up next to it. Nothing loud, just enough to help you keep track of what you've already seen if you're browsing through several.

It resets if you close the tab or come back another day. It's not trying to track you forever, just to help while you're actually looking around.

Here's the prompt that builds this:

Small detail, but it's one of my favorite ones on the whole site.

```text
When a link to a project is clicked, save that project's id into a list in sessionStorage. On the page that lists all the projects, check that saved list against every project shown, and reveal a small hidden badge next to any project whose id is in the list. Keep the badge hidden by default so it only ever appears for something the visitor actually opened.
```

## 2. The short version, before any images

A recruiter gives your case study about 30 seconds before deciding whether to keep reading.

So I stopped making them earn it.

Every one of my 12 case studies now opens with a block called The short version. Three boxes, before any images, before any scrolling.

The problem. What I did. What changed.

Two lines each. That's the whole project. If that's all somebody reads, they still know what the work was and whether it went anywhere.

The long version is still underneath. The research, the wrong turns, the screens. But nobody has to dig through it to find out if the project's even relevant to them.

Here's the part I didn't expect.

Writing two lines for What changed is much harder than writing four paragraphs about process. Process writes itself. An outcome makes you admit whether anything actually moved.

On some projects it didn't, or the numbers were never verified. So the block says that out loud. Exact percentages are left out on purpose, because the analytics behind them was never confirmed.

A portfolio that quietly rounds numbers up is worth less than one that tells you which ones it doesn't trust.

If you want to do this to your own case studies, here's the prompt.

Go read the top of your own case study. Could a stranger tell you what it was in 30 seconds?

```text
Add a short summary block at the top of each of my case studies, before any images. Three parts: The problem, What I did, What changed. Two lines each, plain language, no jargon. Write it so someone who reads only this block still knows what the project was and whether it worked. Where I don't have a verified number for an outcome, say so in one line rather than leaving it vague or estimating.
```

## 3. A selection colour that belongs to the brand

Select some text on my site. It won't be the blue you're used to.

It's the same yellow the pixels use, and that's not a coincidence.

Every browser highlights selected text in the same default blue. It's the one piece of your design the browser picks for you, and most people never touch it.

Mine's a warm yellow with near black text on top. It isn't a new colour though. It's the first of the four accent colours the pixel effects already use on the page, so selecting a sentence quietly reuses something you've already seen.

Here's the part worth stealing.

I didn't write a light version and a dark version. The pair is fixed. Yellow behind, near black in front, in both themes. Because both halves are locked together, the page theme can't break it.

That combination lands at about 13 to 1 contrast, which is far past the accessibility minimum. A selection colour is the easiest place in a design to accidentally make text unreadable, and it's the one nobody tests.

It's two lines of CSS. No JavaScript, no library.

Small thing. It's also the kind of detail that says somebody looked at every corner of the page, not just the parts people expect.

```text
Override the browser's default text selection colour for my whole site. Use an accent colour that already appears elsewhere in my design as the highlight, with a near black text colour on top of it. Set the same fixed pair in both light and dark mode rather than writing a variant for each, so the theme cannot make it unreadable, and check the pair passes contrast for normal text. Include the standard rule and the Firefox prefixed one.
```

---

MIT licensed. Made by [Miguel Clavel](https://miguelclavel.com/?utm_source=github&utm_medium=portfolio-details) with Claude Code.
