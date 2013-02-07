![logo](https://github.com/baskerville/thmkit/raw/master/logo/thmkit_logo.png)

## Usage

    trtpl [OPTIONS] TEMPLATE_DIR
    gencs COLOR_PROFILE

The `TRTPL_FILTERS_DIR` environment variable shall point to the directory holding your custom filters.

## Example Invocation

    TRTPL_FILTERS_DIR=./examples/filters ./trtpl -o output -c examples/color_schemes/raven_dark.yaml examples/templates

## Required Libraries

- python-colormath
- python-jinja2
- python-yaml
