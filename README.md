# Introduction

This is the Youwe coding standard for Magento 2 projects. It is based on
the default Magento2 coding standard but some tests have been removed to create
a workable and fast standard.

# Installation

Use composer to require the standard in a project.

```shell
composer require --dev youwe/coding-standard-magento2
```

To let PHPCS know that this standard should be used add a phpcs.xml file in the
root of the project.

```xml
<?xml version="1.0"?>
<ruleset>
    <rule ref="./vendor/youwe/coding-standard-magento2/src/YouweMagento2"/>
</ruleset>
```

# Integration with PHPStorm and automatic testing

The recommended way to enable the coding standard in PHPStorm and automatic
testing is by requiring the Youwe testing suite in a project.

```shell
composer require --dev youwe/testing-suite
```

For more information go to [Youwe Testing Suite](https://github.com/YouweGit/testing-suite).

# Contribution guidelines

Contributions are welcome. Please create pull requests which add or remove
tests.
