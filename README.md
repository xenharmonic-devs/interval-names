# interval-names

A list of interval names in programmatically readable formats.

## Format

### JSON

An interval is a plain object and the list file contains an array of interval objects.

Here is the format of a single interval object.

```json
{
  "names": [<String>, ...],
  "ratio": [<int>, <int>],
  "cents": <float>
}
```

The interval object has a mandatory `names` field with at least 1 String. It also requires at least one of `cents`
or `ratio`, but both can be defined. `cent` takes a float value and `ratio` takes 2 integers. The integers inside
`ratio` are not ordered.

## Sources

* http://www.tonalsoft.com/enc/i/interval-list.aspx
