# Chapter 2: A Pragmatic Approach

**Notes by Ryan**

### The Essence of Good Design

> Tip 14: Good design is easier to change than bad design

What is this tip trying to say? Software engineering, unlike other forms of engineering, has a special relationship with change. Intentions, requirements, goals, technologies, they all _change_. Are you building for just _business value_ today?

You might have read about the [SOLID principles](https://en.wikipedia.org/wiki/SOLID), and specifically the first, the _Single Responsibility Principle_:

> A class should only have a single responsibility, that is, only changes to one part of the software's specification should be able to affect the specification of the class.

This is a specified use case for _SRP_, but more generally, it's about answering this question:

> What will change _this_ code?

---

The advice of _ETC_ (easier to change), the premise, is that it assumes you can tell _how to make something easier to change_: do you think in practice this is true? What's the balance of abstraction and reusability?

### DRY—The Evils of Duplication

> DRY is about duplication of knowledge

What are your experiences with this principle today?

---

In the code examples in this section, there is a single method, and later, it is _refactored_ into multiple. How does this compare to your approach to refactoring and heading towards _DRY_ code?

---

Have you ever had a code review claim duplication? Was it a situation similar to as it was described in _Not All Code Duplication Is Knowledge Duplication_?

---

Do all methods and functions _need_ documentation? Is there a risk of adding it but not maintaining it?

---

What are the properties of a DRY data structure?

---

When is duplication OK? When is it a _better of two evils_ kind of situation?

### Orthogonality

### Reversibility

### Tracer Bullets

### Prototypes and Post-it Notes

### Domain Languages

### Estimating