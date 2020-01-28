shallowcp
=========

## Build dependencies
- `guile`
- `autoconf`
- `automake`
- `pkg-config`
- `awk`
- `sed`
- `grep`
- `coreutils`

## Run-time dependencies
- `guile`

## Using the build system
```
autoreconf -vif
./configure
```

## Without using the build system

Because the build system introduces a whole list of dependencies, and
manually ``building'' it is quite easy, here are the instructions to
``build'' it without using the build system.

1. Replace `@GUILE` in `shallowcp.in` to your GNU Guile path.
2. Rename `shallowcp.in` to `shallowcp`
3. Give `shallowcp` execute permissions with `chmod +x shallowcp`

## Usage

```
./shallowcp source-dir dest-dir
```
