Changelog 1.2
=============

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this project adheres to 
[Semantic Versioning](http://semver.org/spec/v2.0.0.html).


## [1.2.0 (Summer Smith)](https://github.com/php-censor/php-censor/tree/1.2.0) (2019-xx-xx)

[Full Changelog](https://github.com/php-censor/php-censor/compare/1.1.4...1.2.0)

### Added

- [PhpUnit] Badge for PhpUnit plugin coverage level (shields.io). 
Issue [#306](https://github.com/php-censor/php-censor/issues/306).
- [PhpUnit] Options `required_classes_coverage`, `required_methods_coverage`, `required_lines_coverage`. 
Issue [#299](https://github.com/php-censor/php-censor/issues/299). Pull request 
[#354](https://github.com/php-censor/php-censor/pull/354). Thanks to [@slavkluev](https://github.com/slavkluev).
- [Shell] Option `execute_all` for Shell plugin.
- [MySQL, PostgreSQL, SQLite] Option `options` (For PDO additional options) for plugins MySQL, PostgreSQL and SQLite 
(Optional).
- [MySQL, PostgreSQL] Options `port` and `dbname` for plugins MySQL and PostgreSQL (Optional).
- [MySQL] Option `charset` for plugin MySQL (Optional).
- [PhpTalLint] Options "allowed_errors" and `allowed_warnings`.
- [BitbucketNotify] PhpUnit code coverage for BitbucketNotify. Pull requests 
[#308](https://github.com/php-censor/php-censor/pull/308), [#309](https://github.com/php-censor/php-censor/pull/309), 
[#312](https://github.com/php-censor/php-censor/pull/312), [#323](https://github.com/php-censor/php-censor/pull/323). 
Thanks to [@lugark](https://github.com/lugark).
- Default value for DB port parameter during the installation (`3306` for MySQL and `5432` for PostgreSQL). Issue 
[#316](https://github.com/php-censor/php-censor/issues/316).
- Yaml project config validation for project edit web-interface. Pull requests 
[#332](https://github.com/php-censor/php-censor/pull/332), [#336](https://github.com/php-censor/php-censor/pull/336). 
Thanks to [@lugark](https://github.com/lugark).

### Fixed

- [PHPCodeSniffer] PHPCodeSniffer plugin dependencies for PHP `7.3`. Issue 
[#334](https://github.com/php-censor/php-censor/issues/334). Pull request 
[#335](https://github.com/php-censor/php-censor/pull/335). Thanks to [@xl32](https://github.com/xl32).

### Removed

- Useless installation and configuration option `php-censor.url`.

### Changed

- [PhpCsFixer, PhpDocblockChecker] Improved plugins output. Pull request 
[#357](https://github.com/php-censor/php-censor/pull/357). Thanks to [@SimonHeimberg](https://github.com/SimonHeimberg).
- [SecurityChecker] Now you may use `symfony` binary for security check with option `binary_name` 
(`symfony security:check`). Pull request [#358](https://github.com/php-censor/php-censor/pull/358). Thanks 
to [@SimonHeimberg](https://github.com/SimonHeimberg).
- [PhpUnit] Improved catching coverage output. Pull request [#355](https://github.com/php-censor/php-censor/pull/355). 
Thanks to [@SimonHeimberg](https://github.com/SimonHeimberg).
- Improved code style, documentation and localizations. Pull requests 
[#331](https://github.com/php-censor/php-censor/pull/331), [#330](https://github.com/php-censor/php-censor/pull/330), 
[#329](https://github.com/php-censor/php-censor/pull/329), [#328](https://github.com/php-censor/php-censor/pull/328), 
[#322](https://github.com/php-censor/php-censor/pull/322), [#317](https://github.com/php-censor/php-censor/pull/317), 
[#356](https://github.com/php-censor/php-censor/pull/356), [#361](https://github.com/php-censor/php-censor/pull/361). 
Thanks to [@Ultra9](https://github.com/Ultra9), [@mixo](https://github.com/mixo) 
and [@SimonHeimberg](https://github.com/SimonHeimberg).
- Default value of global configuration param `allow_public_artifacts` (`true` -> `false`).
- Build branch default (`master` -> `master|default|trunk` for `git|hg|svn`).
- **Deprecated**:
    - [PackageBuild] Special variables for plugin PackageBuild (`%build.commit%`, `%build.id%`, `%build.branch%`, 
    `%project.title%`, `%date%` and `%time%`) are deprecated and will be deleted in version 2.0. Use interpolated 
    variables instead (`%COMMIT_ID%`, `%BUILD_ID%`, `%BRANCH%`, `%PROJECT_TITLE%`, `%CURRENT_DATE%`, `CURRENT_TIME`).
    - [Shell] Option `command` and commands list without any named option for plugin Shell are deprecated and will be 
    deleted in version 2.0. Use option `commands` instead.
    - [MySQL and PostgreSQL] Options `pass` for plugins MySQL and PostgreSQL is deprecated will be deleted in version 
    2.0. Use option `password` instead.
    - [MySQL, PostgreSQL, SQLite] Queries list without option for plugins MySQL, PostgreSQL and SQLite is deprecated 
    and will be deleted in version 2.0. Use the options `queries` instead.
    - [MySQL] Imports list without option for plugin MySQL is deprecated and will be deleted in version 2.0. Use 
    the options `imports` instead.
    - [Mage, Mage3] Section `mage` and `mage3` in the global application config and option `bin` is deprecated and 
    will be deleted in version 2.0. Use the plugin options `binary_path` and `binary_name` instead.


## Other versions

- [0.x Changelog](/docs/CHANGELOG_0.x.md)
- [1.0 Changelog](/docs/CHANGELOG_1.0.md)
- [1.1 Changelog](/docs/CHANGELOG_1.1.md)
