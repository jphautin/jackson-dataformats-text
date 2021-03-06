## Overview

This is a multi-module umbrella project for [Jackson](../../../jackson)
standard text-format dataformat backends.

Dataformat backends are used to support format alternatives to JSON, supported
by default. This is done by sub-classing Jackson core abstractions of:

* All backends sub-class `JsonFactory`, which is factory for:
    * `JsonParser` for reading data (decoding data encoding in supported format)
    * `JsonGenerator` for writing data (encoding data using supported format)
* Some backens sub-class `ObjectMapper` for additional support for databinding

## Textual formats included

Currently included backends are:

* [CSV](csv/)
* [Properties](properties/)
* [YAML](yaml/)

Standard supported formats that are not yet included here (but are likely added
in future)  are:

* [XML](../../jackson-dataformt-xml)

## License

All modules are licensed under [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0.txt).

## Status

[![Build Status](https://travis-ci.org/FasterXML/jackson-dataformats-text.svg)](https://travis-ci.org/FasterXML/jackson-dataformats-text)

## More

See [Wiki](../../wiki) for more information (javadocs).
