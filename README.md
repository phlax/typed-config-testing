# typed-config-testing

to test out this schema with `vscode`, first install `vscode-yaml`, next open
your `settings.json` and ensure you have the following in the `yaml.schemas`
section:

```
"yaml.schemas": {
	"https://phlax.github.io/typed-config-testing/example-schema.json": ["example*yaml"]
}
```

Now open a file matching the above pattern - eg `example1.yaml`. You should have
auto-complete following the schema in https://github.com/phlax/typed-config-testing/blob/master/example-schema.json

Add a section as follows:

```
typed_config:
   "@type": "TYPE_NAME"

```

if you set `TYPE_NAME` to one of

- `some.typed_config.type1`
- `some.typed_config.type2`

you should see the autocomplete within the `typed_config` section change.
