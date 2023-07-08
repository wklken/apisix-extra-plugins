# apisix-plugins

unofficial plugin for apisix

## plugins

- [buffered-file-logger](./apisix/plugins/buffered-file-logger.lua): file-logger with batch processor

## usage

according to the [apisix doc: plugin develop](https://apisix.apache.org/docs/apisix/plugin-develop/)

1. `git clone https://github.com/wklken/apisix-extra-plugins.git`
2. `apisix.extra_lua_path =  "/path/to/apisix-extra-plugins/?.lua"` in `conf/config.yaml`
3. enable the plugin by name in `plugins` field of `conf/config.yaml`

```yaml
apisix:
    ...
    extra_lua_path: "/path/to/example/?.lua"
plugins:
  ...
  - buffered-file-logger
```
