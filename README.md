# Very clean code

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

- PHP + SQL: ORM
- PHP + HTML: template engine
- PHP + JavaScript: JSON
- PHP + CSS: use CSS classes and variables

## Principles

- Abstraction: strive to make deeper layers do the work, write less project-specific code.
- Be explicit! Implicit things need more brain work thus are error prone.
