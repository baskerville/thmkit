![logo](https://github.com/baskerville/thmkit/raw/master/logo/thmkit_logo.png)

## Usage

    trtpl [OPTIONS] TEMPLATES_DIR

## Description

`trtpl` renders templates via YAML color schemes and Jinja2 filters.

The directory structure present in the template directory is reproduced in the output directory.

The `JINJA2_FILTERS_DIR` environment variable shall point to the directory holding your custom filters (`trtpl` will try to import `$JINJA2_FILTERS_DIR/trtpl_filters.py`).

## Options

- `-h, --help` — Show the synopsis on standard output and exit.

- `-c, --color-scheme COLOR_SCHEME` — Read colors from the given file.

- `-i, --color-space LCH|Lab|CMYK` — Set the color space of the color scheme.

- `-o, --output-directory OUTPUT_DIR` — Define where the compiled templates will be stored.

- `-s, --filename-suffix SUFFIX` — Add the given suffix to the output file names.

- `-p, --preserve-extensions` — Preserve templates file name extensions in outputs.

## Example Invocation

    JINJA2_FILTERS_DIR=./examples/filters ./trtpl -o output -c examples/color_schemes/ivory-dark.yaml -i LCH examples/templates
    ./output/redef

## Required Libraries

- python-colormath
- python-jinja2
- python-yaml
