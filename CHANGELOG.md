# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 2.1.1
### Changed
- Allow use of stable version of `dealerdirect/phpcodesniffer-composer-installer`

## 2.1.0
### Changed
- Youwe ruleset will not check .phtml files anymore and only uses the Magento2 coding standards to check files on `phpcs`.

## 2.0.0
### Added
- Composer package youwe/coding-standard which is now included in the Youwe coding standards for Magento 2.
- Comments for why the ruleset was added.
- Coding standards for phtml templates.
- Package [magento/magento-coding-standard](https://github.com/magento/magento-coding-standard) as a requirement.
  The version v25 is used as a base. If not compatible please update the `phpcs.xml` in project root.

### Removed
- Rule PSR2.Methods.MethodDeclaration.Underscore since this is already excluded by Magento.
- Argument colors and added it in the common Youwe coding standards.
- Old coding ruleset directories and migrated them to YouweMagento2.

## 1.7.0 - 2021-12-24
### Changed
- Vendor from MediactMagento2 to Magento2
- Copyrights.

### Removed
- Dependency squizlabs/php_codesniffer.
