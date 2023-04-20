# Very clean code

[![Tweet](https://img.shields.io/badge/Tweet-share-d5d5d5?style=social&logo=twitter)](https://twitter.com/intent/tweet?text=Found%20useful%20policies%20of%20%40szepeviktor&url=https%3A%2F%2Fgithub.com%2Fszepeviktor%2Fvery-clean-code)
[![theories](https://img.shields.io/badge/more-theories-purple)](https://github.com/stars/szepeviktor/lists/theory)

Additions to https://github.com/piotrplenik/clean-code-php

## 🟢 Happy and unhappy path

```
if (error) unhappy path;

happy path;
```

🖱️ https://szymonkrajewski.pl/why-should-you-return-early/

## 🟢 Arrays versus objects

An array is a dumb container of unknown data. Arrays should be used to store lists: keyless elements of the same type.
BTW strings are containers of unknown bytes.

🖱️ https://github.com/CuyZ/Valinor

## 🟢 Base value of an array

The base value of an array is not `null` but `[]`.

## 🔴 String manipulation

String manipulation including concatenation is the job of low level libraries as it is highly error prone.
:bulb: Creating messages for UI and logs is not string manipulation.

## 🟢 Write positive conditions

Explicit is better than implicit.

```
❌ if (state !== null)
✔️ if (state instanceof Resolver)
```

## 🔴 Mixing programming languages

Have low-level libraries connect different languages.

- Main language + SQL: ORM
- Main language + HTML: template engine
- Main language + JavaScript: JSON
- Main language + CSS: use CSS classes and CSS variables

## Principles

- Abstraction: strive to make deeper layers do the work, write less project-specific code.
- Be explicit! Implicit things need more brain work thus are error prone.
- > There are only two hard things in Computer Science: cache invalidation and naming things.

    — Phil Karlton

    Gain knowledge of _things_, so you can name them.

## Support my thinking

Please consider supporting my work, as formulating the conclusions above takes at least several months.

[![Sponsor](https://github.com/szepeviktor/.github/raw/master/.github/assets/github-like-sponsor-button.svg)](https://github.com/sponsors/szepeviktor)

Thank you!
