+++
date = '2025-11-27'
draft = true
title = 'Blog Architecture'
+++

Use the "Vault to blog" plugin

At a high-level:
- The blog is hosted on GitHub Pages
- richkuz.net has a CNAME pointing at richkuz.github.io/blog
- I write posts in markdown in Obsidian
- The Obsidian "Remotely Save" plugin backs up my Obsidian vault to an AWS S3 bucket
- A GitHub action pulls the latest .md files from S3 and commits them to the repo
- I already use Obsidian Vault Sync for reliable two-way sync across Mac and Android. Great for daily use, ensuring my desktop and mobile edits work well on the same file together.
- I also configure the "Remotely Save" Obsidian Plugin to backup my vault to an S3 bucket
	- I set the Sync Direction to "Incremental Push And Delete" so it works like a backup clone.
- TODO How can my blog fetch public S3 content?
TODO Configure an IAM role that can only read from the /blog folder in the bucket