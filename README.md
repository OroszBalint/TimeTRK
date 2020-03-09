# TimeTRK

<img src="https://camo.githubusercontent.com/9a140a4c68e7c178bc660bee7675f4f25ff7ade3/68747470733a2f2f696d672e736869656c64732e696f2f6e706d2f6c2f7675652e737667">

Simple timetracking cli with polibar support and pandoc export.

## Dependencies

- dmenu

## Install

``` bash
git clone https://github.com/OroszBalint/TimeTRK.git
cd TimeTRK
chmod +x trk

# add to Path or make alias for it
```

## usage

``` bash
# start timer
trk +

# stop timer
trk -

# echo elapsed time since start (if started)
trk

# print report
trk report
```

## Polybar

``` config
[module/trk]

type = custom/script
exec = ~/path/to/TimeTRK/trk
interval = 1
click-left = ~/path/to/TimeTRK/trk +
click-right = ~/path/to/TimeTRK/trk -

# than add trk to modules
```

## TODO

- [x] dmenu projects
- [x] sum the working hours
- [ ] pandoc or latex monthly export
