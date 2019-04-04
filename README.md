# mozilla-build-configs

### Usage:

```bash
git clone --depth=1 git@github.com:MozillaSecurity/mozilla-build-configs.git
cd mozilla-central # Previously cloned source directory
export MOZCONFIG=../mozilla-build-configs/firefox.asan.fuzzing.release

```

### Optional: Use provided .mozbuild clang version
```
./mach bootstrap
export CC="$HOME/.mozbuild/clang/bin/clang"
export CXX="$HOME/.mozbuild/clang/bin/clang++"
```

### Build
```
./mach build
```


### LibFuzzer Requirement

```bash
./mach gtest nonexistent
```
