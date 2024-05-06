* Lua

  There are three types of my Lua code assemblies.

  First is "workshop", it is my personal Lua framework. Mix of different
  design decisions in my Lua journey. Contains essential pieces for all
  projects I've done.

  Second is "released projects". They are self-contained solutions
  having in repository all the code they need and no dead code. Frozen
  in their time. They have "workshop" directory.

  Third is "unreleased projects". They are considered WIP and so
  expected to grow to "released projects" and get their own "workshop"
  snapshot. I'm mentioning them here mostly for my own convenience, huh.
  They don't have "workshop" directory, so you need to clone that repo
  if you want to tinker with them.

  * [Workshop](https://github.com/martin-eden/workshop)
    (Since 2016-09. But core parts started since my Lua journey, 2013)

    Personal codebase for Lua projects.

    My Lua code hive. That's evolution, not design.

  * [Lua code formatter (lcf)](https://github.com/martin-eden/lua_code_formatter)
    (2016-08/2017-01)

    Parses source text to AST, transforms AST, compiles back to source text.

    Still one of the best projects I've made. Core is my grammar parser
    with two main modes (sequence and choice) and one flag (repeat). Like
    LPEG but different. Also invented and tried many design patters there.

    Satellite projects

    * [Lua table serializer](https://github.com/martin-eden/lua_table_serializer)
      (2017-05)

      Serialize Lua table to source code that recreates this table.

      Tables in Lua can contain cycles, so you can't serialize them to
      data format like JSON. Dealing with cycles was challenging
      challenge.

    * [Autoldoc](https://github.com/martin-eden/autoldoc)
      (2017-08)

      Automatically place LDoc comments in Lua source file.

      Mostly POC, I'm not using auto-documenters as a class. Used AST
      from my code formatter to locate places where to insert
      documentation comments.

    * [Command-line generator for lcf](https://github.com/martin-eden/lcf_params_gui)
      (2018-07)

      GUI to generate Bash command line for Lua code formatter.

      Was playing with TekUI(Lua/C) library.

  * [DS3231 GUI](https://github.com/martin-eden/tekui_ds3231)
    (2019-12/2020-01)

    Graphical interface to hardware real-time clock module DS3231.
    (Hardware host part is Firmata-compatible board.)

    I2C channel from Firmata (in Arduino), USB connection, data
    parser/compiler in Lua and representation of structured data in
    TekUI. Then data goes back on the chain. Was pleasant experience.

  * [Lightday](https://github.com/martin-eden/lightday)
    (2020-03)

    TekUI to calculate length of lightday. (Depending of latitude
    and day number.)

  * [Firmata ambassador](https://github.com/martin-eden/FirmataAmbassador)
    (2023-06)

    Sort of "Ambassador" to do useful things via dreadful Firmata protocol.

    Protocol parser/compiler. Reimplemented in a sane way. I threw my
    previous close-to-protocol implementation and switched focus to
    easy-to-understand interface.

  * [ArduinoLibGenerator](https://github.com/martin-eden/ArduinoLibGenerator)
    (2024-02/2024-03)

    Tool to generate library description file for ArduinoIDE. Source
    data for library description is structured Lua table.

    Yo dawg i herd you dont like writing one-dimensional .ini files,
    not real programmers job?

* Embedded C++: Arduino(ATMega328P) and Esplora(ESP8266)

  * Libraries

    * [me_Types](https://github.com/martin-eden/EmbeddedCpp_me_Types)
      (2024-02)

      Base types for other code.

    * [me_WifiShip](https://github.com/martin-eden/EmbeddedCpp_me_WifiShip)
      (2024-02)

      Esplora. Get/set MAC, scan, connect to router, get IP.

    * [me_Ws2812b docs](https://github.com/martin-eden/EmbeddedCpp-me_Ws2812b-Docs)
      (2024-05)

      Additional docs for WS2812B LED stripe library.

  * [Willy](https://github.com/martin-eden/willy)
    (2023-12, WIP)

    Two wheeled rover.

    Two decks, standoffs, battery, two DC motors, wheels, motor board,
    Arduino, Esplora, gyroscope (IMU6050).

    You can send commands to rover via Internet! (Well, at least in
    you local network). You will receive gyroscope readings as a
    feedback! You can teach this thingie to do tricks!

    Actually, it's good recent project but currently I'm disctracted to
    designing WiFi interface classet in C++. Was not proper announced
    yet.

  * [Sketchbook](https://github.com/martin-eden/arduino_sketchbook)
    (Since 2017-07.)

    Personal codebase for embedded C++ projects.

    Mess of my C sketches/libraries for Arduino. Someday I'll clean this up!
    (Or at least will make it cleaner.)

    That's a lot worse than my Lua "workshop". All code since the dawn
    of 2015s when I started relations with Arduino and was forced to write in
    C/C++. (Was writing in Pascal/Delphi before.)

    But recent libraries there are not bad at experimental design.

* Games

  World of Warcraft and Hearthstone-related side scripts.

  Currently I do not play these games (and Blizzard banned my several
  accounts). But the effort was spend so they are public archives.

  Stack is Lua, Bash (and parallel).

  * [Hearthstone cards renamer](https://github.com/martin-eden/hearthstone_cards_renamer)
    (2018-05)

    * [Hearthstone cards images](https://github.com/martin-eden/hearthstone_cards_named)
      (2018-04)

  * [Warcraft. Retrieve auction data for pets](https://github.com/martin-eden/pet_aux)
    (2016-06)

  * [Warcraft. Get general data about pets](https://github.com/martin-eden/pet_species_to_csv)
    (2016-06)

* Texts

  * [Tagging style](https://github.com/martin-eden/tagging_guideline)
    (2016-07)

    System of marking commit messages.

    Was written by me somewhere in 2016. But still interesting text to
    read if you wonder about syntax in my git commit messages.

  * [Firmata protocol](https://github.com/martin-eden/firmata_protocol/blob/main/protocol.md)
    (2021-08, 2023-05)

    Firmata protocol description. (Firmata protocol is related to Arduino world.)

    I've tried to describe protocol from my conspects and Lua implementations.

  * Minor
    * Reference docs
      * [Zip format](https://github.com/martin-eden/zipfiles_format_doc) - official text docs with my .pdf equivalents
      * [DS3231](https://github.com/martin-eden/doc.ds3231) - datasheet for real time clock chip DS3231

* Links to other resources I value

  * Tools
    * [Lua](https://github.com/lua/lua) - thanks Roberto for elegant language!
      * [LuaGLM](https://github.com/gottfriedleibniz/lua) - math-tuned fork of Lua
    * [FreePascal](https://github.com/fpc/FPCSource)
    * [GNU compilers collection](https://github.com/gcc-mirror/gcc) - thank you Richard for making open-source practical!
    * [linux](https://github.com/torvalds/linux) - thanks Linus for OS core
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
      * [Fengari](https://github.com/fengari-lua/fengari) by `daurnimator` -- run Lua in browser
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
