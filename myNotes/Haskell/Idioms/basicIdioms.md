[[haskell-main]]


Idiom #53 Join a list of strings
```join str = intercalate ", " str```


With Text...

```import qualified Data.Text as T
{-# LANGUAGE OverloadedStrings #-}
y :: T.Text
y = T.intercalate ", " x```

https://programming-idioms.org/idiom/53/join-a-list-of-strings/793/haskell

