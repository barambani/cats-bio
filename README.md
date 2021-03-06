# Cats BIO

A Bifunctorial IO Implementation for Cats based on standard `cats.effect.IO`.


## Benchmarks

The `BIO` included in this repo is `bio`.

`ioEitherT` refers to `EitherT[cats.effect.IO, E, A]`.

The Scalaz bifunctor IO (here nicknamed `zio`) is taken from here: https://github.com/scalaz/ioeffect

```
[info] Benchmark               Mode  Cnt         Score         Error  Units
[info] FlatMapBench.bio        avgt   15   7984481.602 ±  374087.511  ns/op
[info] FlatMapBench.ioEitherT  avgt   15  50550527.610 ± 4696081.849  ns/op
[info] FlatMapBench.zio        avgt   15  11198233.659 ± 1758884.388  ns/op
```
