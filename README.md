# N2O project sample

## Build

```shell
$ export LEAN_HOME=/path/to/lean4
$ export LEAN_PATH=$LEAN_HOME/library:../n2o/src:../nitro/src:./src
$ $LEAN_HOME/bin/lean -c sample.cpp src/sample.lean
$ $LEAN_HOME/bin/leanc sample.cpp ../n2o/libn2o.a ../nitro/libnitro.a -lwebsockets -o sample
$ ./sample
```
