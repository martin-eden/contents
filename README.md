## Parts of my extended phenotype

* Embedded C++: Arduino(ATMega328P) and Esplora(ESP8266)

  Organizing data in convenient way is the hardest challenge I've
  encountered.

  * [Personal framework](https://github.com/martin-eden/Embedded_Crafts/tree/master/Parts)
  * [Crafts](https://github.com/martin-eden/Embedded_Crafts/tree/master/Ships)
  * Featured crafts
    * [me_WifiShip](https://github.com/martin-eden/Embedded-me_WifiShip)
      (2023, 2024) for API design and file structure
    * [me_Ws2812b](https://github.com/martin-eden/Embedded-me_Ws2812b)
      (2024) for writing in assembler and trying to stay readable
    * [Willy](https://github.com/martin-eden/willy)
      (2023, 2024) for creating G-codes-like abstraction for
      motor control, for implementing stack from HTTP to PWM.

* Lua: Stock Lua 5.3

  Here are two types of my Lua code assemblies.

  First is "workshop", it is my personal Lua framework. It's code pieces
  from different times and constantly evolving.

  Second is "released projects". These are self-contained solutions
  without unused code. Typically has part of "workshop" at release time.

  * [Workshop](https://github.com/martin-eden/workshop)
    (2015 .. )

    Personal codebase for Lua projects.

  * [Lua code formatter (lcf)](https://github.com/martin-eden/lua_code_formatter)
    (2016, 2017)

    Full Lua 5.3 syntax parser, formatter and compiler.

    Satellite projects

    * [Lua table serializer](https://github.com/martin-eden/lua_table_serializer)
      (2017)

      Serializes Lua table to source code that recreates that table.

    * [Autoldoc](https://github.com/martin-eden/autoldoc)
      (2017)

      Places LDoc comments in Lua source file.

    * [Command-line generator for lcf](https://github.com/martin-eden/lcf_params_gui)
      (2018)

      GUI to generate Bash command line for Lua code formatter.

  * [DS3231 GUI][DS3231 GUI]
    (2019, 2026)

    GUI to hardware real-time clock module DS3231.

  * [Lightday](https://github.com/martin-eden/lightday)
    (2020)

    GUI to calculate length of lightday (depending of latitude
    and day number).

  * [Firmata ambassador](https://github.com/martin-eden/FirmataAmbassador)
    (2023)

    Simplified support of Firmata communication protocol.

  * [ArduinoLibGenerator](https://github.com/martin-eden/ArduinoLibGenerator)
    (2024)

    Codec for `.properties` library description files in ArduinoIDE.

  * [Itness](https://github.com/martin-eden/Lua-Itness)
    (2024, 2026)

    Strings tree codec.

  * [RgbStripeConsole](https://github.com/martin-eden/Lua-RgbStripeConsole)
    (2024)

    Communication interface to custom firmware for RGB stripe.

  * [Plain pixmap load/save][PlainPixmap]
    (2024)

    Plaintext images format codec (`.pbm`, `.pgm`, `.pbm`, `.ppm`).

  * [Lua code melder (lcm)](https://github.com/martin-eden/lua_code_melder)
    (2024, 2026)

    Aggregates `*.lua` files in directory tree into one.

  * [Linear "plasm" gradient generator][1dPlasm]
    (2024)

    Generates image file with random distance-dependent gradient transitions.

  * [BinToImg][BinToImg]
    (2026)

    Converts any file to image.

  * [I2C_Console][I2C_Console_Client]
    (2026)

    Communication interface to custom firmware for I²C interface.

  * [RangesTree][RangesTree]
    (2026)

    Module to work with data ranges in a tree structure.

* Texts

  * [Tagging style](https://github.com/martin-eden/tagging_guideline)
    (2016)

    System of marking commit messages.

  * [Firmata protocol](https://github.com/martin-eden/firmata_protocol/blob/main/protocol.md)
    (2021, 2023)

    Firmata protocol description.

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
      * [compiled Windows binaries](https://github.com/joedf/LuaBuilds) `LuaBuilds` by `Joe DF`
      * [cryptoroutines](https://github.com/philanc/plc) `plc` by `philanc`
      * [graph planar representation](https://github.com/rm-code/Graphoon) `Graphoon` by `Robert Machmer`
      * [table serializer](https://github.com/gvx/Ser) `Ser` by `gvx`
      * [Lua parser](https://github.com/andremm/lua-parser) by `Andre Murbach`
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

  * Game sources
    * [RedAlert](https://github.com/electronicarts/CnC_Remastered_Collection/blob/master/REDALERT/)
      RedAlert game source, kudos to `Joe L. Bolstic`
    * [Jagged Alliance 2](https://github.com/dariusk/ja2/tree/master/ja2/Build/TacticalAI)
      JA2 source
    * [Descent FreeSpace](https://github.com/osgcc/descent2)
    * [Quake](https://github.com/id-Software/Quake)
    * [Doom](https://github.com/id-Software/DOOM)
    * [Hack](https://cvsweb.netbsd.org/bsdweb.cgi/src/games/hack/)

[DS3231 GUI]: https://github.com/martin-eden/tekui_ds3231
[PlainPixmap]: https://github.com/martin-eden/Lua-Ppm
[1dPlasm]: https://github.com/martin-eden/Lua-LinearPlasmGenerator
[BinToImg]: https://github.com/martin-eden/Lua-BinToImg
[I2C_Console_Client]: https://github.com/martin-eden/Lua-I2C_Console
[RangesTree]: https://github.com/martin-eden/Lua-RangesTree
