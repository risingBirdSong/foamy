[[functions]]
[[MakeArrayConsecutive2]]
length :: forall (t :: * -> *) a. Foldable t => t a -> Int

Returns the size/length of a finite structure as an Int . The default implementation is optimized for structures that are similar to cons-lists, because there is no general way to do better.