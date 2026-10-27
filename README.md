# vipmike007.github.io

Personal site and blog of Mike Cao — https://vipmike007.github.io

## Writing a blog post

1. Copy `_drafts/post-template.md` into `_posts/` and rename it to
   `YYYY-MM-DD-short-title.md` (for example `_posts/2026-11-03-openshift-upgrade-tips.md`).
   The date in the file name is the publish date.
2. Edit the `title`, `description`, and `tags` at the top, then write the post in Markdown below
   the second `---`. `title_zh` / `description_zh` are optional Chinese versions shown when the
   visitor switches to 中文.
   - **One language:** delete the `<div class="en">` / `<div class="zh">` wrappers and just write.
     The post is shown to everyone.
   - **Both languages:** keep the wrappers and put each version in its own block (see the template).
3. Put images in `assets/images/` and reference them as `![alt text](/assets/images/name.png)`.
4. Commit and push to `master`. GitHub Pages rebuilds the site in about a minute; the post appears
   on the home page ("Latest writing") and at https://vipmike007.github.io/blog/.

Files in `_drafts/` are never published, so you can keep unfinished posts there.

You can also write a post directly on GitHub: open the repo, go to `_posts/`, click
**Add file → Create new file**, name it `YYYY-MM-DD-title.md`, paste the template, and commit.

## English / 中文

Every piece of text on the site exists twice: `<span class="en">…</span><span class="zh">…</span>`
(or the same classes on a block element). The EN / 中文 switch in the top bar shows one and hides
the other, and remembers the choice. Link to a specific language with `?lang=en` or `?lang=zh`.

## Preview locally (optional)

```bash
docker run --rm -it -p 4000:4000 -v "$PWD":/site -w /site ruby:3.3 \
  sh -c "bundle install && bundle exec jekyll serve --host 0.0.0.0 --drafts"
```

Then open http://localhost:4000.
