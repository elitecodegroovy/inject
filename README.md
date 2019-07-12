# Inject

Package inject provides a reflect based injector. A large application built with dependency injection in mind will typically involve the boring work of setting up the object graph. This library attempts to take care of this boring work by creating and connecting the various objects. Its use involves you seeding the object graph with some (possibly incomplete) objects, where the underlying types have been tagged for injection. Given this, the library will populate the objects creating new ones as necessary. It uses singletons by default, supports optional private instances as well as named instances.

It works using Go's reflection package and is inherently limited in what it can do as opposed to a code-gen system with respect to private fields. It was fork from `https://github.com/facebookarchive/inject`
