# elinks-basis

basis plugin for elinks plugins
also provides a command prompt which can be used by other plugins.


# install

1. you need to install [elinks-plug](http://github.com/yazgoo/elinks-plug)
1. then you need to add to your hook file the following plugin:

```lua
plug("git@github.com:yazgoo/elinks-basis")
```
# running it

press `:` to get the command prompt.
default available commands are `source`, `update` to update vim-plug

# using it in your plugins 

Adding a custom command (callable via `:`):

```lua
add_command("cmd_name", function(args) do_something() end)
```

Addin a custom pre_format_hook

```lua
add_pre_format_hook("hook_name", function(url, html) return /* something */ end)
```
