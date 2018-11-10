---
title: "Notes"
date: 2018-11-10T13:30:58+10:00
draft: false
headless: true
---

`partials/menus/structure/menu` below recursively iterates over each section, regardless of whether menus are defined for such sections or pages. An asterisk `*` preceding an entry's title denotes that it is a non-section page.

`partials/menus/lazy/menu` follows the documentation for [Section Menu for Lazy Bloggers](https://gohugo.io/templates/menu-templates/#section-menu-for-lazy-bloggers) 

`partials/menus/config/menu` generates menus as configured in the `config.toml` (`.Site.Menus.second`), frontmatter (`.Site.Menus.third`), and lazy menus (`.Site.Menus.main`).

### Some observations:
**Scenario: Lazy Menus with nested sections**