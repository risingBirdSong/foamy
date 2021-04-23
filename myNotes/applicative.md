[[haskell-main]]

how are applicatives monads?  
```hs
ff <*> fa = do
  f <- ff
  a <- fa
  pure (f a)
```
