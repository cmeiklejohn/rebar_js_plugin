# Rebar JS Plugin

Rebar extensions for JavaScript development with Erlang.  Metapackage combining

* [rebar_js_concatenator_plugin](https://github.com/cmeiklejohn/rebar_js_concatenator_plugin)
* [rebar_js_uglifier_plugin](https://github.com/cmeiklejohn/rebar_js_uglifier_plugin)
* [rebar_js_minispade_plugin](https://github.com/cmeiklejohn/rebar_js_minispade_plugin)
* [rebar_js_handlebars_plugin](https://github.com/cmeiklejohn/rebar_js_handlebars_plugin)

## Installation

Specify ```rebar_js_plugin``` as a dependency in your ```rebar.config```.

```erlang
{deps, [
       {rebar_js_plugin, ".*",
        {git, "git://github.com/cmeiklejohn/rebar_js_plugin.git", {branch, "master"}}}
]}.
```

Then, configure your plugins in your ```rebar.config``` with the plugins
you'd like to use.  This module is usageful for getting around rebar
single plugin_dir errors.

```erlang
{plugins, [rebar_js_concatenator_plugin, rebar_js_uglifier_plugin]}.
```
