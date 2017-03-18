# django-optimzations

### tl;dr

This talk revolves around profiling & optimization of Django applications. It aims at accreating performance by optimal usage of Django ORM, in-memory caching & handling resource intensive requests asynchronously using task queues such as Celery.

### Django Optimzations -- What to expect in this talk?

Many amateur developers who picks up Django write code which seems to work, but fails at scale.

Django has been made as a The web framework for perfectionists with deadlines, and perfection is often forgotten due to deadlines. In this talk, we'll discuss about common pitfalls to avoid while working on a Django based web application. The talk would revolve mostly around the following:

    - Profiling our web application to know exactly what queries are being executed on the database.
    - Making optimal use of Django ORM to avoid multiple queries to the database.
    - Usage of F objects, Q objects, prefetch_related, select_related et. all.
    Addressing n+1 queries problems to database with ORM.
    - Making use of Asynchronous requests to avoid creating a backlog for the request-response cycle. A little bit about task queues like Celery.
    - Caching: Different types of caches to use -- both django caching as well as something like in-memory Redis cache.

In the end we'll look at an overall architecture of entire Django web application including wsgi, nginx, caching and database layer. This would provide a starting point to write clean code and optimizing Django Applications to the audience

#### Find the [proposal here](https://cfp.pydelhi.org/pydelhi-conference-2017/proposals/optimizing-django-for-building-high-performance-systems~b68ne/)

This is made using [reveal.js](https://github.com/hakimel/reveal.js). I'm thankful to the creators of Reveal JS.
