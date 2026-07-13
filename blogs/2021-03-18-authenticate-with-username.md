---
title: "Authenticate with username"
url: "https://fury.blog/changelog/2021-03-18-user-token-auth/"
date: "2021-03-18"
author: "hello@gemfury.com (Gemfury Team)"
feed_url: "https://fury.blog/rss/"
---
The long-awaited feature of USER:TOKEN authentication has landed. You can now use the following Repo-URL authentication format: https://USER:TOKEN@repo.fury.io/ACCOUNT ACCOUNT remains the username of the repository, while USER is verified as the owner of the TOKEN . Even if the token is valid, authentication will fail if that username is incorrect.
