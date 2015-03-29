# Writing Partymapper

## 3. Bootstrapping with Composer

Here we go.

`$ mkdir partymapper`

First things first. Let's set this project up with composer:

```json
{
    "name": "partymapper/partymapper",
    "description": "Find parties near you",
    "authors": [
        {
            "name": "Pedro Gil Candeias",
            "email": "pgscandeias@gmail.com"
        }
    ],
    "require": {
        "doctrine/collections": "1.*"
    },
    "require-dev": {
        "phpunit/phpunit": "4.5.*"
    },
    "autoload": {
        "psr-4": {
            "Partymapper\\": "./src",
            "tests\\Partymapper\\": "./tests"
        }
    },
    "config": {
        "bin-dir": "bin"
    }
}
```

`doctrine/collections` is there because I can't be bothered with arrays when it comes to entity associations and `ArrayCollection` is such a sweet little class.

`phpunit/phpunit` is still the alpha and the omega of php unit testing, despite a strong challenge by phpspec. You just can't beat its versatility. Version 4.5 includes Prophecy, meaning mocking is no longer painful.
