# Profiling Python Applications

This repository contains examples on how to profile Python applications using [`cProfile`](https://docs.python.org/3/library/profile.html#module-cProfile), [`snakeviz`](http://jiffyclub.github.io/snakeviz/), [`line_profiler`](https://github.com/pyutils/line_profiler), and [`memory_profiler`](https://pypi.org/project/memory-profiler/) modules.

## Environment setup
To reproduce the same environment, I suggest using [Conda](https://docs.conda.io/projects/conda/en/latest/index.html) as your package manager. If you have it installed, you can use [environment.yml](./environment.yml) to create it using
```bash
conda env create -f environment.yml
```
and activate it with
```bash
conda activate profiling
```

## Profiling
In each example, you will find a `profile.sh` script that will run the Python code with the [`cProfile`](https://docs.python.org/3/library/profile.html#module-cProfile) module on. Running this script will generate a file `example.prof`, that contains the profiling data.


## Visualization
Even though it is possible to get statistics directly from [`cProfile`](https://docs.python.org/3/library/profile.html#module-cProfile), a great way to visualize the profiling results is with [`snakeviz`](http://jiffyclub.github.io/snakeviz/). It's very easy to use. For each example, you will find a `visualize.sh` script that, when run, will launch [`snakeviz`](http://jiffyclub.github.io/snakeviz/) in a browser tab. Have fun!
