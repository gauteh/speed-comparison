# Speed comparison of programming languages

This projects tries to compare the speed of different programming languages.

It uses an implementation of the [Leibniz formula for π](https://en.wikipedia.org/wiki/Leibniz_formula_for_%CF%80) to do the comparison.

Here is a video which explains how it works: [Calculating π by hand](https://www.youtube.com/watch?v=HrRMnzANHHs)

In this project we don't really care about getting a precise calculation of pi. We only want to see how fast are the programming languages doing.

## Run it yourself

Everything is run by a Docker container and a bash script which envokes the programs.
To measure the execution time the command [`time`](https://en.wikipedia.org/wiki/Time_(Unix)) is used.

### Requirements

- `Docker`
- `Makefile` support

### Execute it

Just run: `make`

## Results

```text
======= Comparison =======

> Python 3
Version: Python 3.6.3
Time:
real    0m 0.37s
user    0m 0.37s
sys     0m 0.00s
Result: π = 3.1415936535887745

> PHP7
Version: PHP 7.1.14 (cli) (built: Feb  8 2018 15:10:11) ( NTS )
Copyright (c) 1997-2018 The PHP Group
Zend Engine v3.1.0, Copyright (c) 1998-2018 Zend Technologies
Time:
real    0m 0.05s
user    0m 0.05s
sys     0m 0.00s
Result: π = 3.1415936535887745

> Rust
Version: rustc 1.22.1
Time:
real    0m 0.13s
user    0m 0.12s
sys     0m 0.00s
Result: π = 3.1415936535887745
```

## Thanks

This projects tries to recreate the results which [Thomas](https://www.thomaschristlieb.de) did [on his blog](https://www.thomaschristlieb.de/performance-vergleich-zwischen-verschiedenen-programmiersprachen-und-systemen/).
It also tries to include languages which Thomas didn't cover in his post.
