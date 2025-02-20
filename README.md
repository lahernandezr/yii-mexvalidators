# Yii Mexico Data Validators (yii-mexvalidators)

Validators for two data strings used in Mexico for identity, RFC CURP and IMSS, for use with the [Yii 2.0.* framework][1].

## Installation

Add dependency to your ```composer.json``` file:

```json
{
    "require": {
        "ktaris/yii-mexvalidators": "0.1.1"
    }
}
```

## Usage

In order to use the validator, you need to provide the full path to the validator in the model:

```php
public function rules()
{
    return [
       ['rfc', 'vendor.ktaris.yii-mexvalidators.rfcValidator'],
       ['curp', 'vendor.ktaris.yii-mexvalidators.curpValidator'],
       ['imss', 'vendor.ktaris.yii-mexvalidators.imssValidator'],
    ];
}
```

[1]: https://github.com/yiisoft/yii "Yii Framework"
