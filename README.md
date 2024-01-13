<div align="center">

<img src="https://cdn.discordapp.com/attachments/955362477137362954/996769449480826971/2022-07-13_16-25.png" width="350px">

# `NiTch`

<h3>
  incredibly fast system fetch written in <code>nim👑</code>
</h3>

</div>

# Description 📖

<img src="https://media.discordapp.net/attachments/955362477137362954/997839005460725841/2022-07-16_15-15_1.png" width="42%" align="right">

`nitch` is a small and incredibly fast system fetch written fully in `nim👑` without any dependencies, on my pc
it executes in around 1.70 miliseconds.

The source code of `nitch` is highly documented and I hope it will act as a learning resource for nim
and linux systems architecture

If anything in the source code is unclear or is lacking in its explanation, open an issue. Sometimes you get too close to something and you fail to see the "bigger picture"!


btw written in `nim👑`

why `nim👑`? because it's fast and simple

<br>

# Installation ☁️
Requirements:
- nim
- nimble (usually included with your nim installation)
```fish
nimble install https://github.com/arashi-software/nitch
```

# Usage 🪨
```
nitch
```

flags:
```
Usage:
  nitch
  nitch -h|--help
  nitch -v|--version

Options:
  -h, --help     Show help message
  -v, --version  return version of program
  -a, --ascii    return fetch with ascii art
  -s, --square   return fetch with square corners
```

<br>

# Configuration ⚙️
### `nitch` is configured by changing the source code
### `src/funcs/drawing.nim` - config file

# Building 📦
### 0) install [nim](https://nim-lang.org/)

### 1) clone repo
```fish
git clone https://github.com/unxsh/nitch.git
```
### 2) change dir to `nitch`
```fish
cd nitch/
```

### 3) build program with `nimble`
```fish
nimble build
```
After that you will get a ready-made binary file in the root directory of the project.

<br>

# File architecture 📁
```fish
nitch
├── LICENSE
├── nitch
├── nitch.nimble
├── README.md
├── setup.sh
├── src
│   ├── assets
│   │   ├── assets.nim
│   │   └── logos.nim
│   ├── flags
│   │   └── args.nim
│   ├── funcs
│   │   ├── drawing.nim
│   │   ├── getDistroId.nim
│   │   ├── packages
│   │   │   ├── getDpkgPkgs.nim
│   │   │   ├── getPacmanPkgs.nim
│   │   │   ├── getPortagePkgs.nim
│   │   │   ├── getRpmPkgs.nim
│   │   │   └── getXbpsPkgs.nim
│   │   └── perform.nim
│   ├── nitches
│   │   ├── getDistro.nim
│   │   ├── getHostname.nim
│   │   ├── getKernel.nim
│   │   ├── getLogo.nim
│   │   ├── getPkgs.nim
│   │   ├── getRam.nim
│   │   ├── getShell.nim
│   │   ├── getUptime.nim
│   │   └── getUser.nim
│   ├── nitch.nim
│   └── nitch.nim.cfg
└── templates
    ├── bfetch
    ├── cfgParser.nim
    ├── colorTest.nim
    ├── data.dat
    ├── echo.sh
    ├── listFiles.nim
    ├── readLine.nim
    ├── refTest.nim
    ├── rxfetch
    ├── shellCheck.nim
    ├── slice.nim
    ├── test.cfg
    ├── testCounter.nim
    ├── testFile
    ├── testProc.nim
    └── tupleTest.nim

8 directories, 43 files
```

# Thanks for ideas & examples 💬
- [pfetch](https://github.com/dylanaraps/pfetch/)
- [neofetch](https://github.com/dylanaraps/neofetch)
- [paleofetch](https://github.com/ss7m/paleofetch)
- [rxfetch](https://github.com/Mangeshrex/rxfetch)
- [nerdfetch](https://github.com/ThatOneCalculator/NerdFetch)
