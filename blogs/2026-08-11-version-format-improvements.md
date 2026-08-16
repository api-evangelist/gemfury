---
title: "Version format improvements"
url: "https://fury.blog/changelog/2026-08-11-version-format-improvements/"
date: "2026-08-11"
author: "hello@gemfury.com (Gemfury Team)"
feed_url: "https://fury.blog/rss/"
---
We’ve rolled out a set of improvements to how Gemfury parses and validates package versions. Failed uploads now report version format errors for otherwise valid packages. Often, client-side tooling has little to no validation for version format, and until this update, an upload with an unsupported version would fail with a generic error, leaving you to guess at the cause.
