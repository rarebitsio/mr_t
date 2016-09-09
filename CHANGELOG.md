## CHANGELOG


v0.6.0:
- flexible ExUnit wrapper (lib/runner/config.ex)
- more docs
- new top-level functions
  - MrT.run_all_strategy_on
  - MrT.run_all_strategy_off
  - MrT.focus(:focus)
  - MrT.unfocus
  - MrT.verbosity_on
  - MrT.verbosity_off

v0.5.8:
- run_all / run_matching functions directly on MrT module

v0.5.7:
- less verbosity by default (https://github.com/ruby2elixir/mr_t/pull/3)
- short GIF demo in Readme

v0.5.6:
- fixes a regression bug, MrT.Monitor.Src was not restarted on syntax error, fixed by `MrT.Utils.require_file(file_path)` upfront

v0.5.5:
- much less logic for reloading, overall simpler code

v0.5.4:
- works better with controller tests (the matcher remove _controller from the filename before matching)


v0.5.3:
- turn full recompilation back on (solves https://github.com/ruby2elixir/mr_t/issues/1)
- use the IEx.Helpers recompile function (it seems more robust)
