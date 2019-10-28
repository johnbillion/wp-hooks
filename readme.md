# wp-hooks

WordPress actions and filters in machine-readable JSON format.

**Note:** This is still a work in progress.

## Installation

`composer require johnbillion/wp-hooks=dev-master`

## Actions and Filters

* Actions can be found in [`hooks/actions.json`](hooks/actions.json).
* Filters can be found in [`hooks/filters.json`](hooks/filters.json).

## Schema

* The JSON schema can be found in [`schema.json`](schema.json).

## Implementation Details

The hook extraction component of the [WP Parser library](https://github.com/WordPress/phpdoc-parser) is used to scan files in order to generate the hook data. WordPress nightly is used so hooks are always up to date.

## Regenerating the Hook Files

`composer generate`

## Validating the Hook Files

`composer validate-files`
