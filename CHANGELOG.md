# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 2.2.1
## Fixed
- Exclude pattern, the patterns did not include the dot of the extension allowing matching with the pathname (which for example in DDEV will match with `html` in `/var/www/html`)
## Changed
- Included more rules to exclude for (p)html and xml files. Indentation, line-length are very hard to fix consistently and prevents usage of component libraries (as for example with Hyvä)

## 2.2.0
## Changed
- Apply more rules to .html and .phtml files. In previous updates (see pull requests [#5] and [#10]), we excluded these files very widely; this change makes the exclusion more specific and intentional.

[#5]: https://github.com/YouweGit/coding-standard-magento2/pull/5
[#10]: https://github.com/YouweGit/coding-standard-magento2/pull/10

## 2.1.3
### Fixed
- Youwe ruleset will not check .html files any more. See also version 2.1.0.

## 2.1.2
### Changed
- Allow use of stable version of `dealerdirect/phpcodesniffer-composer-installer`

## 2.1.1
### Fixed
- Resolve incompatibility with `PSR12.ControlStructures.ControlStructureSpacing` (from the `Youwe` standard) and `PSR2.ControlStructures.ControlStructureSpacing` (from the `Magento2` standard).
  For details, see https://github.com/YouweGit/coding-standard-magento2/issues/6.

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
