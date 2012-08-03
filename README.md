# Rebar JS Plugin

Rebar extensions for JavaScript development with Erlang.  Metapackage
combining the
[rebar_js_concatenator_plugin](https://github.com/cmeiklejohn/rebar_js_concatenator_plugin)
and the
[rebar_js_uglifier_plugin](https://github.com/cmeiklejohn/rebar_js_uglifier_plugin).

## Installation

Specify ```rebar_js_plugin``` as a dependency in your ```rebar.config```.

```erlang
{deps, [
       {rebar_js_plugin, ".*",
        {git, "git://github.com/cmeiklejohn/rebar_js_plugin.git", {branch, "master"}}}
]}.
```

Then, configure your plugins in your ```rebar.config```.

```erlang
{plugin_dir, "deps/rebar_js_plugin/src"}.
{plugins, [rebar_js_concatenator_plugin, rebar_js_uglifier_plugin]}.
```
