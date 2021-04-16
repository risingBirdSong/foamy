https://wiki.haskell.org/Language_Pragmas
[[haskell-main]]
### Example
(top of file)
```
{-# LANGUAGE OverloadedStrings #-}
{-# LANGUAGE TemplateHaskell #-}
```

Language pragmas can be combined into a comma-separated list:

```{-# LANGUAGE OverloadedStrings, TemplateHaskell #-}```