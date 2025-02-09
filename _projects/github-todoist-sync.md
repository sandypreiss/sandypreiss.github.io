---
title: "GitHub-Todoist syncer"
collection: projects
category: personal
permalink: /project/github-todoist-sync
excerpt: "Lightweight utility to sync GitHub issues and Todoist tasks."
date: 2025-01-01
venue:
repourl: https://github.com/sandypreiss/github-todoist-sync
appurl:
paperurl:
citation:
---

For various reasons, my team at RTI doesn't have a unified task management platform. Many of our projects use GitHub issues for task management. Others use Teams, and others nothing at all. We can't always control this, because we work with lots of groups across the company. Most of them aren't developers. And our projects are often a small component of much bigger projects, which already have their task management approaches set.

Many of my teammates use Todoist to keep a unified to-do list. It's a great app, but entering tasks requires a lot of manual effort.

I created this utility to automate some of that manual effort. It connects our Todoist accounts to our GitHub organization. As issues are opened, assigned, and closed, it automatically creates and closes Todoist tasks.