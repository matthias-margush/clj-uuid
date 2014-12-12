# clj-uuid

A Clojure library for generation and utilization of UUIDs (Universally
Unique Identifiers) as described by RFC-4122. This library extends the
standard Java UUID class to provide true v1 (time based) and v3/v5
(namespace based) identifier generation. Additionally, a number of
useful supporting utilities are provided to support serialization and
manipulation of these UUIDs in a simple, efficient manner.

The essential nature of the value RFC4122 UUIDs provide is that of an
enormous namespace and a deterministic mathematical model by means of
which one navigates it. UUIDs represent an extremely powerful and
versatile computation technique that is often overlooked, and
underutilized. In my opinion, this, in part, is due to the generally
poor quality, performance, and capability of available libraries and,
in part, due to a general misunderstanding in the popular consiousness
of their proper use and benefit. It is my hope that this library will
serve to expand awareness, make available, and simplify use of RFC4122
identifiers to a wider audience.

## How Big?

The provided namespace represents an _inexhaustable_ resource and as
such can be used in a variety of ways not feasible using traditional
techniques rooted in the notions imposed by finite resources.  When I
say "inexhaustable" this of course is slight hyperbolie, but not by
much.  The upper bound on the representation implemented by this
library limits the number of unique identifiers to a mere...

*three hundred forty undecillion two hundred eighty-two decillion three*
*hundred sixty-six nonillion nine hundred twenty octillion nine hundred* 
*thirty-eight septillion four hundred sixty-three sextillion four hundred*
*sixty-three quintillion three hundred seventy-four quadrillion six hundred*
*seven trillion four hundred thirty-one billion seven hundred sixty-eight*
*million two hundred eleven thousand four hundred and fifty-five.*

If you think you might be starting to run low, let me know when you get down
to your last few undecillion or so and I'll see what I can do to help out.


## Motivation

To a large extent, the design of the algorithmic
implementation is inspired by the Common-Lisp library
[_UNICLY_](http://github.com/mon-key/unicly) which is a painstakingly
optimized, encyclopaedic implementation of RFC-4122 the author of
which, Stan Pearman, has devoted considerable effort to research, refine, and
improve.  To my knowledge there is no more performant  and
precise implementation of the RFC-4122 specification available
anywhere, in any language, on any platform.

That having been said, this library intends to present a slightly more
comfortable public interface that places a little more priority on
convenient DWIM semantics at the cost of somewhat less emphasis on
low level performance optimizations.  Since this library is built as
an extension to the standard java.util.UUID class whose implementation
largely dominates its performance characteristics anyway, this seems to
be a reasonable philosophy.

## License

Copyright © 2013 Dan Lentz

Distributed under the Eclipse Public License either version 1.0 

## Usage

### The Most Recent Release

With Leiningen:

```clj
[danlentz/clj-uuid "0.0.7-SNAPSHOT"]
```

With Maven:

```xml
<dependency>
  <groupId>danlentz</groupId>
  <artifactId>clj-uuid</artifactId>
  <version>0.0.6-SNAPSHOT</version>
</dependency>
```



