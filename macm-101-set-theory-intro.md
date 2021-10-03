# macm-101-set-theory-intro

## ZF Set Theory

The natural numbers are defined recursively by letting ```0 = {}``` be the empty set.

```n + 1 = n u {n} for each n```

---

Membership - does an item belong to a set? Must be unambiguous.

Uppercase letters for sets, lowercase letters for elements. (a belongs to A)

We use curly brackets to denote sets, like python: A = {a,b,c}

Sets may be unordered and still be the same.

Sets may not repeat unless they are a MULTI SET. Otherwise you may not have repetition.

---

## Symbols

a ∈ A - 'a' is a member of set 'A'

a ∉ A - 'a' is NOT a member of set 'A'

---

Sets can be equal to each other, subsets, or PROPER subsets.

Sets are equal if they have exactly the same elements (A = B)

If all the members of set A are also members of set B. Denoted using ⊆.

```NOTE: A SET IS A SUBSET OF ITSELF```

If you do not want a set to be a subset of itself then A may be a PROPER SUBSET of B iff A is a subset of B, but B is NOT a subset of A. Denoted with ⊂.

{1,2,3} ⊆ {2,3,1}

{1,2,3} ⊂ {1,2,3,4}

---

Not a subset: ⊄

A ⊄ B

---

## Cardinality 

If a set S and n distinct elements for some natural number n, n is the cardinality (size) of S and S is a finite set. The cardinality of S is denoted by | S |.

ex: ```|S| where S = {3,2,1} is 3```

A set is finite if it has the same cardinality of some natural number n (it is not infinite).

A set is said to be countable if it is the range of an infinite one to one sequence.

There exist uncountable sets.

---

## Power Set

ONLY APPLIES TO A NORMAL SET NOT A MULTI SET

The power set of a set, A, is the set of all subsets of A, denoted by P(A).

```ex: Given A = {1,2} then P(A) = { {}, {1}, {2}, {1,2} }``` 

Notice in the above example that {1,2} == A. So P(A) contains A. P(A) also contains the empty set!

### Cardinality

For any set A with cardinality = n, if n >= 0, A has 2^n subsets. Therefore |P(A)| = 2^n.

---

# Universal Set

A set which has all the elements in the universe of discourse. 

```ex: A question is talking about all positive integers. So the question's universal set is Z+```

---

# Disjoint Sets

If two sets have NO elements in common, they are disjoint sets.

```ex: Set Q and set R-Q would be disjoint, as by definition they have no elements in common```

---



