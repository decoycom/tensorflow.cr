# tensorflow.cr

Crytal binding for [TensorFlow](https://github.com/tensorflow/tensorflow).

## Requiments

You need to compile and install `libtensorflow.so` from [this repo](https://github.com/tensorflow/tensorflow/).

Quick instructions:

```
$ ./configure
$ bazel build :libtensorflow.so
$ cp ./bazel-bin/tensorflow/libtensorflow.so /usr/local/lib/ libtensorflow.so
```

Optional things for OS X:

```
$ install_name_tool -id /usr/local/lib/libtensorflow.so /usr/local/lib/libtensorflow.so
```

## Installation

Add this to your application's `shard.yml`:

```yaml
dependencies:
  tensorflow:
    github: fazibear/tensorflow.cr
```

## Usage

```crystal
require "tensorflow"
```

## Contributing

1. Fork it ( https://github.com/fazibear/tensorflow/fork )
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create a new Pull Request

## Contributors

- [fazibear](https://github.com/fazibear) Michał Kalbarczyk - creator, maintainer