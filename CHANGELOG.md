# Ansigraph Changelog

## Version 0.3

* Reexport the `Color` and `ColorIntensity` data types from `ansi-terminal` for full use of the range of ANSI colors without importing that package.

## Version 0.2

* Improved method of displaying animations so that successive frames overwrite previous ones instead of generating many pages of output. This requires the addition of the `graphHeight :: Graphable a => a -> Int` type class method.

* Improved matrix graphing. Now there are distinct colors to represent positive and negative values, as well as real versus imaginary components. Examples added.

* The `Coloring` data type representing possible terminal colorings has been changed to take `Maybe AnsiColor`s, where `Nothing` indicates use of the default terminal colors.

* Some names have been changed for greater clarity and consistency.

* Dependency bounds updated for GHC 8.

## Version 0.1

Initial release.
