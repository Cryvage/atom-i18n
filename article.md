# Article

## Date

  - 2017-01-18

## Description

  - misc thoughts about this project

## notes


### motivation, before repo init
  - as a user, hope Atom can be better
  - i want to have experience running an open source project
  - Somebody is doing but it can be better
      - current i18n package is only single language
      - can we create a package loading content from different source?
  - Somebody need it
      - several language is missing i18n on [issue](https://github.com/atom/atom/issues/3103)
      - also there are some volunteer for i18n


### Tech Aspect
  - current i18n project
      - `atom-japanese-menu`
          - base
          - with 80% content extracted from code
      - `atom-cht-menu`
          - base on `atom-japanese-menu`
          - more complete coverage of i18n
          - code is more complex
      - both not complicated but with one work to do
          - extracted content from code
  - i fork `atom-japanese-menu` and start to extract content from code
      - discover how UI dom is structured
  - features i want to add
      - common data structure for different lang
      - translate more UI items


### Maintenance Aspect
  - From TODO to Github *Projects*
      - former way: use plain text `TODO.md` to create TODO List
      - issue is always a good way to manage *actions*
      - Why use *Projects*
          - keeping update `TODO.md` is distracting
              - we need something that we can edit see it changed on the fly
          - there are some tiny *chores* no need to add issue number on it
              - e.g. refactor some function, add blabla to README.md
          - there are some abstract ideas need to be noted
          - We need a higher view to manage the project
              - like what trello did
              - practice kanban?
              - You can reference issue in kanban
  - add CI hook to repo to save time reviewing commit
  - issues
      - use label to classify issues


### Public Relation Aspect
  - for volunteer
      - how to find them?
          - atom discussion, issue page
      - prepare `CONTRIBUTING.md` guide
          - refine instruction to let anyone can understand it
          - simplify the process of translation
              - prepare template
              - use prefix to notice what to translate
      - in the PR discussion
          - thank them
      - add volunteer name in `README.md`
  - for user
      - promote your package in Atom discussion
      - get feedback from user
          - add reload prompt notice when switching language
