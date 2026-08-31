## Parts of my extended phenotype

Organizing data in a convenient way is the hardest challenge I've encountered.

* Embedded C++: Arduino(ATmega328P) and Esplora(ESP8266)

  * [Personal framework][embedded_workshop]
  * [Crafts][embedded_crafts]
  * Featured crafts
    * [me_WifiShip][me_WifiShip]
      (2023, 2024) for API design and file structure
    * [me_Ws2812b][me_Ws2812b]
      (2024) for writing in assembler and staying readable
    * [Willy][Embedded_Willy]
      (2023, 2024) for creating G-codes-like abstraction for
      motor control, for implementing stack from HTTP to PWM.

* Lua: Lua 5.3

  Here are two types of my Lua code assemblies.

  First is "workshop", it is my personal Lua framework. It's code pieces
  from different times and constantly evolving.

  Second is "released projects". These are self-contained solutions
  without unused code. Typically they contain part of "workshop" at
  release time.

  | Created | Updated | Name                                               | Description                                                                 | Tags                                           |
  |:-------:|:--------|:--------------------------------------------------:|:----------------------------------------------------------------------------|:----------------------------------------------:|
  |  2015   | 2026    | [Workshop][workshop]                               | Personal codebase for Lua projects.                                         | `framework`                                    |
  |  2017   | 2026    | [Lua table serializer (lts)][lua_table_serializer] | Serializes Lua table to Lua source code that recreates that table.          | `source-tool` `exploration-tool`               |
  |  2024   | 2026    | [Lua code melder (lcm)][lcm]                       | Aggregates `*.lua` files in directory tree into one.                        | `source-tool`                                  |
  |  2026   | 2026    | [Lua code callgraph][LuaCallgraph]                 | Creates execution graphs from any Lua code.                                 | `source-tool` `exploration-tool`               |
  |  2026   | 2026    | [BinToImg][BinToImg]                               | Converts any file to image.                                                 | `exploration-tool`                             |
  |  2024   | 2026    | [Netpbm codec][PlainPixmap]                        | Plaintext images format codec (`.pbm`, `.pgm`, `.pbm`, `.ppm`).             | `data-format`                                  |
  |  2019   | 2026    | [DS3231 GUI][DS3231 GUI]                           | GUI to hardware real-time clock module DS3231 via Firmata.                  | `gui` `communication` `firmata` `I²C` `ds3231` |
  |  2024   | 2026    | [Itness][Itness]                                   | Strings tree codec.                                                         | `custom-data-format`                           |
  |  2026   | 2026    | [RangesTree][RangesTree]                           | Module for data ranges in a tree structure.                                 | `data-structure`                               |
  |  2026   | 2026    | [I2C_Console][I2C_Console_Client]                  | Communication with custom firmware providing I²C interface.                 | `communication` `custom-firmware` `I²C`        |
  |  2024   | 2024    | [Linear "plasm" gradient generator][1dPlasm]       | Generates image file with random distance-dependent gradient transitions.   | `image` `exploration-tool`                     |
  |  2024   | 2024    | [RgbStripeConsole][RgbStripeConsole]               | Communication with firmware providing RGB stripe access.                    | `communication` `custom-firmware`              |
  |  2024   | 2024    | [ArduinoLibGenerator][ArduinoLibGenerator]         | Codec for `.properties` library description file in ArduinoIDE.             | `data-format` `arduino`                        |
  |  2023   | 2023    | [Firmata ambassador][FirmataAmbassador]            | Simplified interface to Firmata communication protocol.                     | `communication` `firmata`                      |
  |  2020   | 2020    | [Lightday][lightday]                               | GUI to calculate length of lightday (depending of latitude and day number). | `gui` `exploration-tool`                       |
  |  2018   | 2018    | [Command-line generator for lcf][lcf_params_gui]   | GUI to generate Bash command line for Lua code formatter.                   | `gui` `exploration-tool`                       |
  |  2017   | 2017    | [Autoldoc][autoldoc]                               | Places LDoc comments in Lua source file.                                    | `source-tool`                                  |
  |  2016   | 2017    | [Lua code formatter (lcf)][lcf]                    | Full Lua 5.3 syntax parser, formatter and compiler.                         | `source-tool` `lua-parser` `lua-formatter`     |

* Texts

  * [Tagging style][tagging_style]
    (2016)

    System of marking commit messages.

  * [Firmata protocol][firmata_protocol]
    (2021, 2023)

    Firmata protocol description.

## Links to other resources I value

  * Tools
    * [Lua][tools_lua] - thanks Roberto for elegant language!
    * [FreePascal][tools_freepascal] - what a pity Anders was bought by Microsoft
    * [GNU compilers collection][tools_gcc] - thanks Richard for making open-source practical!
    * [git][tools_git] - thanks Linus for implementation of versioned filesystem
    * [linux][tools_linux] - thanks Linus for OS core!

  * Lua
    * Tools, libraries
      * [lhf's tools][luatools_lhf] from language coauthor, `Luiz Henrique de Figueiredo`
      * [graph planar representation][luatools_graphoon] `Graphoon` by `Robert Machmer`
      * [compiled Windows binaries][luatools_winbins] `LuaBuilds` by `Joe DF`
      * [cryptoroutines][luatools_crypto] `plc` by `philanc`
      * [table serializer][luatools_table_serializer] `Ser` by `gvx`
      * [Lua parser][luatools_parser] by `Andre Murbach`
    * Transpilers
      * [Fengari][luaimpl_fengari] by `daurnimator` -- run Lua in browser!
      * [LuaJIT][luaimpl_luajit] by `Mike Pall` -- performance-oriented Lua v5.2
    * Language resources, FAQs, link collections
      * [Lua FAQ][luaintro_steve] by `Steve Donovan`
      * [Lua glossary][luaintro_dirk] by `Dirk Laurie ♰`
      * [links collection][luaintro_links_lewis] by `Lewis J Ellis`
      * [code style guide][luaintro_style_olivine] by `Olivine Labs` group

  * Other good people repositories
    * [capnproto][nice_capnproto] data serializer by `Kenton Varda`
    * [luanacha][nice_luanacha] cryptoroutines in C by `philanc`
    * [rhash][nice_rhash] hashes in C by `Alexey Kravchenko`

  * Game sources
    * [Jagged Alliance 2][games_ja2]
    * [RedAlert][games_redalert] Kudos to `Joe L. Bolstic`
    * [Descent 2][games_descent2]
    * [Quake][games_quake]
    * [Doom][games_doom]
    * [Hack][games_hack]

[embedded_workshop]: https://github.com/martin-eden/Embedded_Crafts/tree/master/Parts
[embedded_crafts]:   https://github.com/martin-eden/Embedded_Crafts/tree/master/Ships

[me_WifiShip]:    https://github.com/martin-eden/Embedded-me_WifiShip
[me_Ws2812b]:     https://github.com/martin-eden/Embedded-me_Ws2812b
[Embedded_Willy]: https://github.com/martin-eden/willy

[workshop]:             https://github.com/martin-eden/workshop
[DS3231 GUI]:           https://github.com/martin-eden/tekui_ds3231
[lcm]:                  https://github.com/martin-eden/lua_code_melder
[Itness]:               https://github.com/martin-eden/Lua-Itness
[RangesTree]:           https://github.com/martin-eden/Lua-RangesTree
[BinToImg]:             https://github.com/martin-eden/Lua-BinToImg
[I2C_Console_Client]:   https://github.com/martin-eden/Lua-I2C_Console
[1dPlasm]:              https://github.com/martin-eden/Lua-LinearPlasmGenerator
[RgbStripeConsole]:     https://github.com/martin-eden/Lua-RgbStripeConsole
[PlainPixmap]:          https://github.com/martin-eden/Lua-Ppm
[ArduinoLibGenerator]:  https://github.com/martin-eden/ArduinoLibGenerator
[FirmataAmbassador]:    https://github.com/martin-eden/FirmataAmbassador
[lightday]:             https://github.com/martin-eden/lightday
[lcf]:                  https://github.com/martin-eden/lua_code_formatter
[lcf_params_gui]:       https://github.com/martin-eden/lcf_params_gui
[autoldoc]:             https://github.com/martin-eden/autoldoc
[lua_table_serializer]: https://github.com/martin-eden/lua_table_serializer
[LuaCallgraph]:         https://github.com/martin-eden/Lua-Callgraph

[tagging_style]:    https://github.com/martin-eden/tagging_guideline
[firmata_protocol]: https://github.com/martin-eden/firmata_protocol/blob/main/protocol.md

[tools_lua]:        https://github.com/lua/lua
[tools_freepascal]: https://github.com/fpc/FPCSource
[tools_gcc]:        https://github.com/gcc-mirror/gcc
[tools_git]:        https://github.com/git/git
[tools_linux]:      https://github.com/torvalds/linux

[luatools_lhf]:              http://webserver2.tecgraf.puc-rio.br/~lhf/ftp/lua/
[luatools_graphoon]:         https://github.com/rm-code/Graphoon
[luatools_winbins]:          https://github.com/joedf/LuaBuilds
[luatools_crypto]:           https://github.com/philanc/plc
[luatools_table_serializer]: https://github.com/gvx/Ser
[luatools_parser]:           https://github.com/andremm/lua-parser

[luaimpl_fengari]: https://github.com/fengari-lua/fengari
[luaimpl_luajit]: https://github.com/LuaJIT/LuaJIT

[luaintro_steve]:         https://github.com/stevedonovan/luafaq
[luaintro_dirk]:          https://html-preview.github.io/?url=https://github.com/dlaurie/lua-notes/raw/refs/heads/master/glossary.html
[luaintro_links_lewis]:   https://github.com/LewisJEllis/awesome-lua
[luaintro_style_olivine]: https://github.com/Olivine-Labs/lua-style-guide

[nice_capnproto]: https://github.com/sandstorm-io/capnproto
[nice_luanacha]:  https://github.com/philanc/luanacha
[nice_rhash]:  https://github.com/rhash/RHash

[games_ja2]:      https://github.com/dariusk/ja2
[games_redalert]: https://github.com/electronicarts/CnC_Remastered_Collection/
[games_descent2]: https://github.com/osgcc/descent2
[games_quake]:    https://github.com/id-Software/Quake
[games_doom]:    https://github.com/id-Software/DOOM
[games_hack]:     https://cvsweb.netbsd.org/bsdweb.cgi/src/games/hack/
