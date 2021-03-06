# outlook report mailappusageversionsusercounts

Gets the count of unique users by Outlook desktop version.

## Usage

```sh
m365 outlook report mailappusageversionsusercounts [options]
```

## Options

`-h, --help`
: output usage information

`-p, --period <period>`
: The length of time over which the report is aggregated. Supported values `D7,D30,D90,D180`

`-f, --outputFile [outputFile]`
: Path to the file where the report should be stored in

`--query [query]`
: JMESPath query string. See [http://jmespath.org/](http://jmespath.org/) for more information and examples

`-o, --output [output]`
: Output type. `text,json`. Default `text`

`--verbose`
: Runs command with verbose logging

`--debug`
: Runs command with debug logging

## Examples

Gets the count of unique users by Outlook desktop version for the last week

```sh
m365 outlook report mailappusageversionsusercounts --period D7
```

Gets the count of unique users by Outlook desktop version for the last week and exports the report data in the specified path in text format

```sh
m365 outlook report mailappusageversionsusercounts --period D7 --output text > "mailappusageversionsusercounts.txt"
```

Gets the count of unique users by Outlook desktop version for the last week and exports the report data in the specified path in json format

```sh
m365 outlook report mailappusageversionsusercounts --period D7 --output json > "mailappusageversionsusercounts.json"
```
