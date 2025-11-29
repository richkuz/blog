+++
date = '2025-11-27'
draft = false
title = 'Blog Setup'
+++


### High-Level Setup

- This blog uses the Hugo static site generator with the [hugo-theme-minima](https://github.com/mivinci/hugo-theme-minima) theme.
- I host this blog on GitHub Pages under `richkuz.github.io/blog`
- `richkuz.net` has a `CNAME` record pointing `www` at `richkuz.github.io.`
- I write posts in Obsidian in markdown format
- I push Obsidian markdown files into my [https://github.com/richkuz/blog](GitHub blog repo) using my [github-push-folder Obsidian plug-in](https://github.com/richkuz/github-push-folder)


### Why Hugo over Jekyll?

I like [al-folio](https://github.com/alshedivat/al-folio) on Jekyll, but Hugo has faster build times and there's less to install. Jesse Wei's [blog post](https://jessewei.dev/blog/2023/papermod/) about switching from Hugo with PaperMod to Jekyll almost made me reconsider. But Hugo has momentum, I expect it will improve over time, and gain more mind share. Both systems use markdown, so this feels like a [two-way-door decision](https://www.aboutamazon.com/news/company-news/2016-letter-to-shareholders). It should be easy enough to migrate to another system if needed.

### Other Obsidian plugins evaluated

- [Obsidian Git Plugin](https://github.com/Vinzent03/obsidian-git) - This might work, but it's overkill for my needs and might not work well on Android. Also it performs two-way sync and I only want one-way sync because I use the official Obsidian Sync to keep my files synced across devices.
-  [Vault to blog Plugin](https://github.com/barkstone2/vault-to-blog)  - This might work too, but it looked slightly more restrictive than what I needed.
- [Remotely Save Plugin](https://github.com/remotely-save/remotely-save) - I started with this approach, using it to backup my vault to an AWS S3 folder. But there were several issues:
	- I didn't want two-way syncing, only one-way syncing.
	- I set the Sync Direction to "Incremental Push And Delete", but it didn't reliably delete from S3
	- I didn't want to maintain the added complexity of an IAM role to write to the S3 bucket, plus a GitHub action to periodically poll from S3 with another IAM read role just to update a content folder.
