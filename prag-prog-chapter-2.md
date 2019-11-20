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

This _Orthogonality_ concept comes from Vectors. Can you think of anything else in your programming efforts that are related to this _Vector_ concept as well?

---

It's easy to get caught up in Orthogonality's practice of "promotes reuse". Should a controller be reused? Should a CSV parser be reused?

What happens when the result of two orthogonal components are used together usefully - is it OK to formalize that relationship and have a new "first class" component using both?

---

> If I dramatically change the requirements behind a particular function, how many modules are affected?

The examples given are changing a button in a GUI, adding a special context menu, or using an API to flip between serving a static screen view and separate mobile views. These are generic high level examples of requirement changes. Can you think of more? Can you think of a change so dramatic that you could not salvage what you had before?

---

For you Java developers out there, EJB (Enterprise Java Beans) serve a purpose but they do so "declaratively as annotations". What's a downside of this?

### Reversibility

In this section, this answers the previously asked...

> Can you think of a change so dramatic that you could not salvage what you had before?

Flexible architecture, using interfaces, promoting the orthogonal way, keeping things DRY, all are things to help.

---

What are some current day fads?

### Tracer Bullets

What is your threshold for considering something "that hasn't been built before"?

Exercising small chunks of separate "layers" - why is this a good approach?

---

> Tracer code is not disposable: you write it for keeps.

Do you agree with this?

In _Trace bullets don't always hit their target_, it's argued that you'll "generate a new, more accurate version quickly". Is this accurate?

What's the difference between this and a prototype?

Can you use the _tracer_ approach in conjunction with the _prototype_ approach?

### Prototypes and Post-it Notes

> Its value lies not in the code produced but in the lessons learned.

> Tip 21: Prototype to Learn

How does this compare to what we try to do?

How does this compare with the _tracer_ approach?

### Domain Languages

Why does this section feel strange here?

YAML, JSON - pros and cons?

What's interesting about `gradle` files?

### Estimating

In addition to _units_ in your estimation, what else might be considered from your audience's perspective?

How formally should you estimate? In _Keep track of you estimating prowess_, it argues that you should track your estimations over time and learn from hits and misses. Do you agree with that, and how formal should you go?

Estimation is a political tool as well. How do you keep all parties happy with an estimate?

Estimating eventually leads you to _story points_ and _velocity_...

Read this: [Stop Using Story Points](https://www.industriallogic.com/blog/stop-using-story-points/)
Read this: [Estimation is Evil](https://pragprog.com/magazines/2013-02/estimation-is-evil)
Read this: [Story points](https://ronjeffries.com/articles/019-01ff/story-points/Index.html)

(Am I slightly biased?)