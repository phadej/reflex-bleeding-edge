# reflex-bleeding-edge

Reflex with newer dependencies.

To use add to your `cabal.project`:

```
source-repository-package
  type: git
  location: https://github.com/phadej/reflex-bleeding-edge.git
  -- remember to update
  tag: 029759d45cc3d423cfedaedf061de36b8f7bb582
  subdir: reflex reflex-dom-core patch monoidal-containers

-- haskell-src-exts is expensive
constraints: reflex -use-template-haskell
constraints: haskell-src-exts <0

-- newer dependencies
-- copy allow-newer: lines from cabal.project in this repository.
```
