[[typeclasses]]

```class Eq a => Ord a where```

The Ord class is used for totally ordered datatypes.

Instances of Ord can be derived for any user-defined datatype whose constituent types are in Ord. The declared order of the constructors in the data declaration determines the ordering in derived Ord instances. The Ordering datatype allows a single comparison to determine the precise ordering of two objects.