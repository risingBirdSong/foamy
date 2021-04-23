[[challenges]]
[[maximum]]
[[zipWith]]
[[tail]]
# adjacentElementsProduct

<!-- https://app.codesignal.com/arcade/intro/level-2/xzKiBHjhoinnpdh6m -->
adjacentElementsProduct xs = maximum $ zipWith (*) xs (tail xs)