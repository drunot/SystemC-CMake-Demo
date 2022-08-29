# SystemC CMake Demo

## Setup SystemC

- Download [SystemC](https://systemc.org/resources/standards/). (Select _"SystemC x.x.x - Core SystemC Language (incl TLM and examples)"_)
- Unpack the `*.tar.gz` and make a build folder for CMake inside root of the unpacked file system.
- From the build folder run

```shell
$ CMake ..
```

### Linux

- Make the project

```shell
$  make -j config=Release
```

- With **root privileges** install SystemC

```shell
$  make install config=Release
```

### Windows

- Make the project

```powershell
$  cmake --build . --config Release
```

- With **admin privileges** install SystemC

```powershell
$  cmake --build . -t install --config Release
```

## Run test project

- Clone repo and build as normal with CMake.
- Expected output:

```

        SystemC 2.3.3-Accellera --- Aug 29 2022 12:17:09
        Copyright (c) 1996-2018 by all Contributors,
        ALL RIGHTS RESERVED
Hello World SystemC
```

- (For better intellisense change `includePath` in `.vscode/c_cpp_properties.json` on linux)
