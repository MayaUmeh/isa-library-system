# Item Sharing Association Library System

A Java application for a community library where members can borrow and share items such as books, DVDs and magazines. Built as a **four person team project** for my Computer Science degree at the University of Hertfordshire.

This repository contains **my part of the system**: the core item class hierarchy that the rest of the team built on.

## My contribution

```
Item (abstract)
├── Book
├── DVD
└── Magazine
```

| File | What it does |
|---|---|
| `Item.java` | Abstract base class holding the fields and behaviour every lendable item shares |
| `Book.java` | Book specific details, extends Item |
| `DVD.java` | DVD specific details, extends Item |
| `Magazine.java` | Magazine specific details, extends Item |

## Why I designed it this way
- **Inheritance:** shared details live once in `Item`, so there is no repeated code across item types.
- **Polymorphism:** the rest of the system can treat every item simply as an `Item`, whatever type it is.
- **Easy to extend:** adding a new item type (for example a board game) means writing one new subclass, without changing any existing code.

## Teamwork
We split the system into parts, with each person owning their own section, and brought the work together through a shared GitHub repository. My classes were the foundation that the rest of the team's code was built on.

## Tech
Java · Object oriented design · Git and GitHub

---
[Website](https://mayaumeh.com) · [LinkedIn](https://www.linkedin.com/in/maya-c-umeh-450a91308)
