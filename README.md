# AxonGeek Setup

## Windows 

<a href="windows.md">WSL2 + Ubuntu + ZSH Setup</a>

## Erlang Installation 

Livebook and Axon require Erlang OTP 24 to work. If you are using WSL, it's okay to just download it to Windows. 

<a href="https://www.erlang.org/downloads">Download Erlang</a>

## Elixir Installation

The Elixir installer usually would bundle the Erlang OTP 22 if you skipped the previous step. This would cause issue down the road. 

<a href="https://elixir-lang.org/install.html">Download Elixir</a>

## Python 3 

If you're a Data Science person you should already have this installed but here's a link if you are still stuck in the Python 2 Era

<a href="https://www.python.org/downloads/">Download Python</a>

### Python WSL2 

```bash
sudo apt-get install python-is-python3
sudo apt install python3-pip
pip install numpy
```

## Bazel

Bazel is a build tool to help compile code. You will likely not touch this after its done.

```bash
sudo apt update && sudo apt install bazel-3.7.2
```

## Livebook

After all of these setup work are done we can now proceed to getting Livebook working!

```bash
sudo apt install erlang-inets erlang-os-mon erlang-runtime-tools erlang-ssl
```

### WSL2 adding escript to PATH

```bash
code ~/.zshrc
```

Add the following to the bottom of the file

```bash
export PATH="${PATH}:/root/.mix/escripts"
```
