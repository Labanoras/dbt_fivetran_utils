# dbt_fivetran_utils v0.2.9

## Under the Hood
- Added a specific Snowflake macro designation for the `json_extract_path` macro. ([#50](https://github.com/fivetran/dbt_fivetran_utils/pull/50))
    - This Snowflake version of the macro includes a `try_parse_json` function within the `json_extract_path` function. This allows for the macro to succeed if not all fields are a json object that are being passed through. If a field is not a json object, then a `null` record is generated. 

# dbt_fivetran_utils v0.2.8

## 🚨 Breaking Changes
- n/a

## Bug Fixes
- n/a

## Features
- Added this changelog to capture iterations of the package!
- Added the `add_dbt_source_relation()` macro, which passes the `dbt_source_relation` column created by `union_data()` to `source_relations()` in package staging models. See the README for more details on its appropriate usage.

## Under the Hood
- n/a