[[functions]]
[[palindrome]]

# reverse

## definitions

reverseList = go []
    where
        go acc [] = acc
        go acc (x:xs) = go (x:acc) xs

reverseList = foldl (flip (:)) []

reverse_foldr :: [a] -> [a]  
reverse_foldr s = foldr (\x xs -> xs ++ [x]) [] s 

reverse_foldl :: [a] -> [a]  
reverse_foldl s = foldl (\xs x -> x:xs) [] s 


