---
title: "Notes"
date: 2018-11-10T13:30:58+10:00
draft: false
---

`partials/menus/structure/menu` below recursively iterates over each section, regardless of whether menus are defined for such sections or pages. An asterisk `*` preceding an entry's title denotes that it is a non-section page.

`partials/menus/lazy/menu` follows the documentation for [Section Menu for Lazy Bloggers](https://gohugo.io/templates/menu-templates/#section-menu-for-lazy-bloggers) 

`partials/menus/config/menu` generates menus as configured in the `config.toml` (`.Site.Menus.second`), frontmatter (`.Site.Menus.third`), and lazy menus (`.Site.Menus.main`).

### Scenario
Lazy Menus with nested sections

### Docs
> This will create a menu with all the sections as menu items and all the sections’ pages as “shadow-members”. The shadow implies that the pages isn’t represented by a menu-item themselves, but this enables you to create a top-level menu like this: ...

### Observations


- ~~Only the bottom-most sub-`Section` gets created in the menu~~
- Originally I thought the above, however that is only true in the `Plants` main section, in which `Bryophytes` (2.1.1) is the menu generated. If it were universally true, the `Animals` main section should get `Acoelomates` (1.1.1.1), instead it gets `Deutorostomia` (1.1.1.3).
- If there are multiple sub-sections of the same depth, only one gets created.



---
