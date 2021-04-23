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

```haskell
mapPragma pragmas = "{-# " <> (intercalate " , " $ map (drop 1) (words pragmas)) <> " #-}"

cleanPragma str = dropWhile (\x -> x /= '-') str

-- doesnt remove qoutes, but the do io monad below does
-- convertCMDLineToFilePragma = id . mapPragma . cleanPragma

-- https://stackoverflow.com/questions/12102874/haskell-suppress-quotes-around-strings-when-shown
convertCMDLineToFilePragmaDo str = do
    let cleaned = cleanPragma str
    let mapped = mapPragma cleaned
    putStrLn $ id mapped
```
src ->
/Users/peter/codingHome/haskell/catchall/myGeneralParsingPractice/myParsingPractice
repo -> 
https://github.com/risingBirdSong/parsingCatchall.git