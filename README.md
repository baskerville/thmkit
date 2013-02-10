![logo](https://github.com/baskerville/thmkit/raw/master/logo/thmkit_logo.png)

## Usage

    trtpl [OPTIONS] TEMPLATE_DIR

The `JINJA2_FILTERS_DIR` environment variable shall point to the directory holding your custom filters (`trtpl` will try to import `$JINJA2_FILTERS_DIR/trtpl_filters.py`).

## Options

- `-h, --help` — Show the synopsis on standard output and exit.

- `-c, --color-scheme COLOR_SCHEME` — Read colors from the given file.

- `-i, --color-space LCHab|Lab|CMYK` — Set the color space of the color scheme.

- `-o, --output-directory OUTPUT_DIR` — Define where the compiled templates will be stored.

- `-s, --filename-suffix SUFFIX` — Add the given suffix to the output file names.

- `-p, --preserve-extensions` — Preserve templates file name extensions in outputs.

## Example Invocation

    JINJA2_FILTERS_DIR=./examples/filters ./trtpl -o output -c examples/color_schemes/raven_dark.yaml examples/templates

## Required Libraries

- python-colormath
- python-jinja2
- python-yaml
