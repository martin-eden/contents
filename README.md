## Parts of my extended phenotype

* Embedded C++: Arduino(ATMega328P) and Esplora(ESP8266)

  Organizing data in convenient way is the hardest challenge I've
  encountered.

  * [Crafts](https://github.com/martin-eden/Embedded_Crafts/)
  * Featured crafts
    * [me_WifiShip](https://github.com/martin-eden/Embedded-me_WifiShip)
      (2023-12 .. 2024-02) for API design and file structure
    * [me_Ws2812b](https://github.com/martin-eden/Embedded-me_Ws2812b)
      (2024-03 .. 2024-05) for writing in assembler and trying to stay readable
    * [Willy](https://github.com/martin-eden/willy)
      (2023-11 .. 2024-02 ..) for creating G-codes-like abstraction for
      motor board. For implementing stack from HTTP endpoint to writing
      PWM. And for hardware design.

* Lua: Stock Lua 5.3

  Here are two types of my Lua code assemblies.

  First is "workshop", it is my personal Lua framework. Mix of different
  design decisions in my Lua journey. Contains essential pieces for all
  projects I've done (including abandoned projects).

  Second is "released projects". They are self-contained solutions
  having in repository all the code they need and no dead code. Frozen
  in their time. They have their own "workshop" directory.

  * [Workshop](https://github.com/martin-eden/workshop)
    (2016-09 .. )

    Personal codebase for Lua projects.

    My Lua code hive. That's evolution, not design.

  * [Lua code formatter (lcf)](https://github.com/martin-eden/lua_code_formatter)
    (2016-08 .. 2017-01)

    Parses source text to AST, transforms AST, compiles back to source text.

    Still one of the best projects I ever made. Core is my grammar parser
    with two main modes (sequence and choice) and one flag (repeat). Like
    LPEG but different. Also invented and tried many design patters there.

    Satellite projects

    * [Lua table serializer](https://github.com/martin-eden/lua_table_serializer)
      (2017-05)

      Serialize Lua table to source code that recreates that table.

      Tables in Lua can contain cycles, so you can't serialize them to
      data format like JSON. Dealing with cycles was interesting.

    * [Autoldoc](https://github.com/martin-eden/autoldoc)
      (2017-08)

      Automatically place LDoc comments in Lua source file.

      Mostly POC, I'm not using auto-documenters as a class of tools.
      Used AST from my code formatter to locate places where to insert
      documentation comments.

    * [Command-line generator for lcf](https://github.com/martin-eden/lcf_params_gui)
      (2018-07)

      GUI to generate Bash command line for Lua code formatter.

      Was playing with TekUI(Lua/C) library.

  * [DS3231 GUI][DS3231 GUI]
    (2019-12 .. 2020-01)

    Graphical interface to hardware real-time clock module DS3231.
    (Firmware is Firmata.)

    I2C channel from Firmata (on Arduino) -- USB connection -- data
    parser/compiler in Lua -- representation in TekUI.
    Then data goes back. Was pleasant experience.

  * [Lightday](https://github.com/martin-eden/lightday)
    (2020-03)

    TekUI to calculate length of lightday. (Depending of latitude
    and day number.)

    I was going to use calculations to emulate Sun for my tomatoes
    growbox but plain 16/8 worked better. And you will have troubles
    moving lamp in circle in growbox anyway.

  * [Firmata ambassador](https://github.com/martin-eden/FirmataAmbassador)
    (2023-06)

    Sort of "ambassador" to do useful things via dreadful Firmata protocol.

    Protocol parser/compiler. Reimplemented in a sane way. I threw my
    previous close-to-protocol implementation (used in [DS3231 GUI][DS3231 GUI])
    and switched focus to easy-to-understand interface.

  * [ArduinoLibGenerator](https://github.com/martin-eden/ArduinoLibGenerator)
    (2024-02 .. 2024-03)

    Generate library description file for ArduinoIDE. Source data for
    library description is Lua table.

    Yo dawg i herd you dont like writing one-dimensional .ini files,
    not real programmers job?

    Toy project to hone source files placement skill.

  * [Itness](https://github.com/martin-eden/Lua-Itness)
    (2024-07 .. 2024-09)

    Strings tree coder/decoder to Lua tables.

    Because I want sane readable format. Not JSON, YAML or XML.

    Looks like Lisp code? That's a convergent evolution!

  * [RgbStripeConsole](https://github.com/martin-eden/Lua-RgbStripeConsole)
    (2024-09)

    Commands generator and file sender for firmware on Arduino with RGB stripe.

  * [Plain pixmap load/save][PlainPixmap]
    (2024-11)

    "Plain .ppm" format codec.

  * [Lua code melder (lcm)](https://github.com/martin-eden/lua_code_melder)
    (2024-11)

    Aggregates `*.lua` files into one. Loading modules will still work.

  * [Linear "plasm" gradient generator][1dPlasm]
    (2024-11)

    Generates image file with sometimes pleasantly semi-random gradient transitions.

* Texts

  * [Tagging style](https://github.com/martin-eden/tagging_guideline)
    (2016-07)

    System of marking commit messages.

    Was written in a couple of hours somewhere in 2016. Still
    interesting text to read if you wonder about syntax in my git
    commit messages.

  * [Firmata protocol](https://github.com/martin-eden/firmata_protocol/blob/main/protocol.md)
    (2021-08, 2023-05)

    Firmata protocol description. (Firmata protocol is related to Arduino world.)

    I've tried to describe protocol from my notes and Lua implementations.

## Links to other resources I value

  * Tools
    * [Lua](https://github.com/lua/lua) - thanks Roberto for elegant language!
    * [FreePascal](https://github.com/fpc/FPCSource) - what a pity Anders was bought by Microsoft
    * [GNU compilers collection](https://github.com/gcc-mirror/gcc) - thanks Richard for making open-source practical!
    * [linux](https://github.com/torvalds/linux) - thanks Linus for OS core!
    * [git](https://github.com/git/git) - thanks Linus for implementation of versioned filesystem

  * Lua
    * Tools, libraries
      * [lhf's tools](http://webserver2.tecgraf.puc-rio.br/~lhf/ftp/lua/) from language coauthor, `Luiz Henrique de Figueiredo`
      * [compiled Windows binaries](https://github.com/WinLua/bin) `WinLua` by `Russel Halley`
      * [cryptoroutines](https://github.com/philanc/plc) `plc` by `philanc`
      * [graph planar representation](https://github.com/rm-code/Graphoon) `Graphoon` by `Robert Machmer`
      * [table serializer](https://github.com/gvx/Ser) `Ser` by `gvx`
      * [lua parser](https://github.com/andremm/lua-parser) by `Andre Murbach`
    * Transpilers
      * [Fengari](https://github.com/fengari-lua/fengari) by `daurnimator` -- run Lua in browser!
      * [LuaJIT](https://github.com/LuaJIT/LuaJIT) by `Mike Pall` -- performance-oriented Lua v5.2
    * Language resources, FAQs, link collections
      * [Lua FAQ](https://github.com/stevedonovan/luafaq) by `Steve Donovan`
      * [Lua glossary](https://rawgit.com/dlaurie/lua-notes/master/glossary.html) by `Dirk Laurie ♰`
      * [links collection](https://github.com/LewisJEllis/awesome-lua) by `Lewis J Ellis`
      * [code style guide](https://github.com/Olivine-Labs/lua-style-guide) by `Olivine Labs` group

  * Other good people repositories
    * [data serizalizer](https://github.com/sandstorm-io/capnproto) `canproto` by `Kenton Varda`
    * [cryptoroutines in C](https://github.com/philanc/luanacha) `luanacha` by `philanc`
    * [hashes in C](https://github.com/rhash/RHash/tree/master/librhash) by `Alexey Kravchenko`

[DS3231 GUI]: https://github.com/martin-eden/tekui_ds3231
[PlainPixmap]: https://github.com/martin-eden/Lua-Ppm
[1dPlasm]: https://github.com/martin-eden/Lua-LinearPlasmGenerator
