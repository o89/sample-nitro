# N2O project sample

## Build

First, build [N2O](https://github.com/o89/n2o) and [NITRO](https://github.com/o89/nitro).

```shell
$ export LEAN_HOME=/path/to/lean4
$ export LEAN_PATH=$LEAN_HOME/library:../n2o/src:../nitro/src:./src
$ $LEAN_HOME/bin/lean -c sample.cpp src/sample.lean
$ $LEAN_HOME/bin/leanc sample.cpp ../n2o/libn2o.a ../nitro/libnitro.a -lwebsockets -o sample
$ ./sample
```
