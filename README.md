# Your Wedding Website

Built with [jekyll-theme-easy-wedding](https://github.com/cnorick/jekyll-theme-easy-wedding).

## Quick Setup

### 1. Install Ruby & Jekyll

If you don't have Ruby installed:
- **Mac:** `brew install ruby` (requires [Homebrew](https://brew.sh))
- **Windows:** Use [RubyInstaller](https://rubyinstaller.org/)
- **Linux:** `sudo apt-get install ruby-full`

### 2. Install dependencies

```bash
gem install bundler
bundle install
```

### 3. Run locally

```bash
bundle exec jekyll serve
```

Then open [http://localhost:4000](http://localhost:4000).

---

## Customization Checklist

### _config.yml
- [ ] Update `title` to your names (e.g. `Alex & Jordan`)
- [ ] Update `email`, `url`, `description`

### _data/couple.yml
- [ ] Set `short_name`, `long_name`, and `role` for both partners

### _data/events.yml
- [ ] Update ceremony date/time (ISO 8601 with UTC offset)
- [ ] Update all venue addresses, names, and Google Maps URLs
- [ ] Add/remove events as needed

### _data/settings.yml
- [ ] Replace `hero_image` with your own photo (add to `assets/img/`)
- [ ] Update `post_address` with your RSVP endpoint
- [ ] Adjust `primary_color` to match your wedding palette
- [ ] Choose whether to enable `use_code` for invite codes

### _data/navigation.yml
- [ ] Comment out pages you don't want yet

### _data/faq.yml
- [ ] Replace all placeholder Q&As with your own

### _data/people.yml
- [ ] Add wedding party members and families
- [ ] Add photos to `assets/img/people/`

### _data/registries.yml
- [ ] Update with your real registry URLs

### _stories/
- [ ] Replace placeholder story content with your own
- [ ] Add cover images to `assets/img/` and update paths

### assets/img/
- [ ] Add `hero.jpg` (main homepage background)
- [ ] Add headshots to `assets/img/people/`

---

## Pages
| File | URL | Purpose |
|---|---|---|
| `index.html` | `/` | Home — hero + our story |
| `celebrations.html` | `/celebrations` | Event schedule |
| `people.html` | `/people` | Wedding party |
| `details.html` | `/details` | Venue, hotels, transport |
| `faq.html` | `/faq` | Frequently asked questions |
| `registry.html` | `/registry` | Gift registries |
| `photo-gallery.html` | `/photo-gallery` | Photos |

To hide a page, just remove it from `_data/navigation.yml` (it still exists but won't be linked).

---

## Deploying

The easiest options:
- **GitHub Pages** — push to a `gh-pages` branch; free and automatic
- **Netlify** — connect your repo; auto-deploys on every push (also handles RSVP forms!)
- **Cloudflare Pages** — similar to Netlify

For GitHub Pages, set `baseurl` in `_config.yml` to your repo name if not using a custom domain.
