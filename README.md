# evision
OpenCV-Elixir bindings

## Dependencies

- [OpenCV](https://github.com/opencv/opencv)
- [CMake](https://cmake.org/)

## Installation

In order to use `evision`, you will need Elixir installed. Then create an Elixir project via the `mix` build tool:

```sh
$ mix new my_app
```

Then you can add `evision` as dependency in your `mix.exs`. At the moment you will have to use a Git dependency while we work on our first release:

```elixir
def deps do
  [
    {:evision, "~> 0.1.0-dev", github: "cocoa-xu/evision", branch: "main"}
  ]
end
```

### Todo

- [ ] Update `.py` files in `py_src` so that they output header files for Erlang bindings.
- [ ] Automatically generate `erl_cv_nif.ex` and other `opencv_*.ex` files using Python.
