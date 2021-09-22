[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)

Generate Swagger Documentation from Insomnia REST Client

## How to use it

See usage with:

```
$ openapi-gen --help
```

Generate Swagger documentation:

```
$ openapi-gen generate -insomnia INSOMNIA_EXPORTED_FILE -config CONFIG_FILE -output FORMAT
```

| Option    | Description                                                                       |
| --------- | --------------------------------------------------------------------------------- |
| -insomnia | Insomnia exported file                                                            |
| -config   | API Global Configuration file (see [Configuration Format](#configuration-format)) |
| -output   | Insomnia output format (json or yaml, default json)                               |

## Example

Issue the following command:

```
$ openapi-gen generate -i examples/watchnow.json -c examples/config.json -o json
```

## Configuration Format

```
{
  "title" : "API Name",
  "version" : "API version",
  "host" : "API URL",
  "basePath" : "Base URL",
  "schemes" : "HTTP protocol",
  "description" : "API description"
}
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
