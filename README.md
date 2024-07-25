# npm-scss-utils
NPM package containing my SCSS utils

```bash
$ npm i @aersosi/scss-utils
```

```scss
@use '@aersosi/scss-utils' as utils;

$number: 3.123456789px;
$digits: 4;
$mode: ceil;

@debug "is-number: #{utils.is-number($mode, '$mode')}";
@debug "is-unitless-number: #{utils.is-unitless-number($number, '$number')}";
@debug "is-string: #{utils.is-string($digits,'$digits')}";

@debug "decimal-round: #{utils.decimal-round($number, $digits, $mode)}";

```


