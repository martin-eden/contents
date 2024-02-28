* Lua

  There are three types of my Lua code assemblies.

  First is "workshop", it is my personal Lua framework. Mix of different
  design decisions in my Lua journey. Contains essential pieces for
  all projects I've done.

  Second is "released projects". They are self-contained solutions having in
  repository all the code they need and no dead code. Many are experimental,
  some are utilitarian.

  Third is "unreleased projects". I'm not considering them ready to be
  released but they are still public, I don't have any private repos.
  Some are abandoned/frozen, some are alive. If you want to try them,
  you need to clone "workshop" too.

  * [Lua code formatter (lcf)](https://github.com/martin-eden/lua_code_formatter)

    Parses source text to AST, transforms AST, compiles back to source text.

    Released somewhere in 2016 but still one of the best projects I've
    made. Tried many invented design patterns there. And also the
    general program workflow is not trivial.

    Satellite projects

    * [Lua table serializer](https://github.com/martin-eden/lua_table_serializer)

      Serialize Lua table to text. Text is source code that recreates this table.

      Tables in Lua can contain cycles, so you can't serialize them to
      data format like JSON. Describing cycles was interesting
      challenge.

    * [Autoldoc](https://github.com/martin-eden/autoldoc)

      Automatically place LDoc comments in Lua source file.

      Was using AST from my code formatter to scan it for context and for
      places to insert comments.

    * [Command-line generator for lcf](https://github.com/martin-eden/lcf_params_gui)

      GUI to generate Bash command line for Lua code formatter.

      Was playing with TekUI(Lua/C) library. Has wrappers over library but code is abandoned.

  * [DS3231 GUI](https://github.com/martin-eden/tekui_ds3231)

    Graphical interface to hardware real-time clock module DS3231.
    (Hardware host part is Firmata-compatible board.)

    Playing with I2C channel from Arduino (Firmata), implementing module
    state parser/compiler in Lua and linking structured data to UI
    (via TekUI). Was pleasant experience.

  * [Firmata ambassador](https://github.com/martin-eden/FirmataAmbassador)

    Sort of "Ambassador" to do useful things via dreadful Firmata protocol.

    Harnessing Firmata protocol. Protocol parser/compiler. Reimplemented
    in a sane way.

    I don't like Firmata protocol design. I threw my previous
    close-to-protocol implementation and switched focus to
    easy-to-understand interface.

  * [Lightday](https://github.com/martin-eden/lightday)

    TekUI to calculate length of lightday. (Depending of latitude
    and day number.)

  * [Workshop](https://github.com/martin-eden/workshop)

    Personal codebase for Lua projects.

    My Lua code hive. That's evolution, not design.

* Embedded C++: Arduino(ATMega328P) and Esplora(ESP8266)

  * Libraries

    * [me_Types](https://github.com/martin-eden/EmbeddedCpp_me_Types)

      Base types for other code.

    * [me_WifiShip](https://github.com/martin-eden/EmbeddedCpp_me_WifiShip)

      Esplora. Get/set MAC, scan, connect to router, get IP.

  * [Willy](https://github.com/martin-eden/willy)

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

    * [Hearthstone cards images](https://github.com/martin-eden/hearthstone_cards_named)

  * [Warcraft. Retrieve auction data for pets](https://github.com/martin-eden/pet_aux)

  * [Warcraft. Get general data about pets](https://github.com/martin-eden/pet_species_to_csv)

* Texts

  * [Tagging style](https://github.com/martin-eden/tagging_guideline)

    System of marking commit messages.

    Was written by me somewhere in 2016. But still interesting text to
    read if you wonder about syntax in my git commit messages.

  * [Firmata protocol](https://github.com/martin-eden/firmata_protocol/blob/main/protocol.md)

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
