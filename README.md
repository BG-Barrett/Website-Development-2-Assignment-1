# Wild Welfare

Website Development 2, Assignment One. A website for Wild Welfare, a fictional animal welfare charity, built with Astro and Sass.

| Page | File | What it does |
|---|---|---|
| Home | `src/pages/index.astro` | Introduces the site and shows the time card |
| Animals | `src/pages/animals.astro`, `src/components/AnimalsContent.astro` | Shows, adds, deletes and searches the animals |
| About | `src/pages/about.astro` | Shows information about me, the data and the image credits |

To run the site locally, use `npm run dev`.

## What's left to do

Work through these in order.

### 1. Styling

- [ ] **Animal cards:** give them a background, padding and shadow so they match the Our Work cards. The `$card-` tokens are ready to use.
- [ ] **Animal status:** style the status text, as `.animals__status` has no styles yet. It could use a different colour for each status.
- [ ] **Add animal form:** make the form look like a distinct area, separate from the search row.
- [ ] **About page:** style the "About me" and "About the data" sections, as they're plain text at the moment. Style the stats and credits lists too.
- [ ] **Time card:** give it a background and padding. `.time__card` has a `border-radius`, but you can't see it without a background.
- [ ] **More Info button:** centre the text, which currently sits at the top of the button.

### 2. Spacing

- [ ] **Animals summary:** add space between the "Showing 14 animals" line and the cards.
- [ ] **About headings:** add space below the headings, which sit tight against the text and the credits button.
- [ ] **Credits list:** add space between the button and the list.
- [ ] **Time card section:** reduce the padding, as the `.section` class adds a lot for one line of text.
- [ ] **Sign-up form labels:** add a space between the label and "(required)", which currently reads "Name(required)".
- [ ] **Animal cards:** replace the hard-coded `gap: 1rem` and `0.75rem` with tokens. `$animals-grid-gap` and `$animals-name-spacing` already exist.
- [ ] **Last row of cards:** check the width, as the last two cards are slightly wider than the rest.

### 3. Bug fixes

- [ ] **Species of only spaces:** the add form still accepts this and creates a card with no species. Check `species` as well as `name` in `AnimalsContent.astro`.
- [ ] **Footer link hover:** check the links can still be read on hover. `$footer-link-color-hover` is `$color-primary-200`, which may be too pale for the footer background.
- [ ] **Page description:** replace "Astro description" in `BaseHead.astro` with a real description.
- [ ] **Sign-up button:** it keeps saying "Thanks for signing up!" after the form resets. Decide whether it should change back.
- [ ] **Empty list message:** deleting every animal shows "No animals match your search", even with no search. Decide whether it needs a different message.
- [ ] **Reduced motion:** `FeaturedWork.astro` sets the image `transition` outside the reduced motion check as well as inside it, so the animation always runs. Remove the first one.
- [ ] **Leftover code:**
  - Remove the empty `[data-type="review"]` rule in `Card.astro` and the empty `[data-type="centered"]` rule in `CtaPanel.astro`.
  - Remove the extra `gap: 1rem` in `Card.astro`.
  - Remove the unused `Button` import in `SiteHeader.astro`.
  - Delete `public/images/logo.svg` if nothing uses it.

### 4. Before submitting

- [ ] **Flexbox on Home:** ask the lecturer whether Home's Grid layouts are OK. The spec says each page's structure should use Flexbox, and Home's main layouts mostly use Grid.
- [ ] **Commit and push:** the time card must be included, as it's the main JavaScript on the Home page.
- [ ] **Deploy to Netlify:** then test all three pages on the live site, including add, delete and search.
- [ ] **Image credits:** check the photographer names, add Pixabay as the source, and add the elephant logo.
- [ ] **CA1 Checklist:** fill in the comments for each rubric row. Don't use the footer year as evidence, as it runs at build time rather than in the browser.
- [ ] **AI and sources disclosure:** list the tools, prompts and dates, and include the comments and this README, which Claude Code added on 5 Nov 2026.
- [ ] **Due date:** confirm it on Moodle.
- [ ] **Submit:** put the URL and the checklist on Moodle.
- [ ] **Interview:** make sure you can explain every part of the code.

## Credits

Built from the Astro + Sass starter template (no scoped styles) from the final module of [Beyond CSS](https://beyondcss.dev). Image credits are on the About page.
