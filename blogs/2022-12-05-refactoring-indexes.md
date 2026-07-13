---
title: "Refactoring indexes"
url: "https://fury.blog/changelog/2022-12-05-new-backend/"
date: "2022-12-05"
author: "hello@gemfury.com (Gemfury Team)"
feed_url: "https://fury.blog/rss/"
---
We’ve rebuilt portions of backend index generation and delivery to address recent scaling issues. The resulting reduction in both latencies and errors means faster and more stable installs, especially for customers with larger repositories. A few weeks ago, our team noticed that generation and delivery of larger repository indexes would occasionally cause noteable spikes in 500 and 403 responses from our servers.
