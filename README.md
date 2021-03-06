# Foreword

This repository is a mirror of the code of SymBA* 2 (64-bits)
planner from IPC-2014.

The original link is 
[here](https://fai.cs.uni-saarland.de/torralba/software.html).


# SymBA*

SymBA is built on top of the [Fast Downward](http://www.fast-downward.org/) 
Planning System, so it is made available under the GNU
Public License (GPL).

Note: If you're using the [FD-lab](http://lab.readthedocs.io/en/latest/) 
scripts to run experiments,
there are a couple of things that have to be changed (in case that you
run the planner calling the plan script that we provide you can ignore
all this). We made changes on the translator and preprocessor so you
cannot re-use the preprocessed files from another planners. Also, the
preprocessor needs to receive "--opt-ordering" as parameter. Our plan
script already does that, but using FD-lab will skip that part so a
workaround is needed (e.g, modify the code of preprocess to put
opt-ordering to true as default).
