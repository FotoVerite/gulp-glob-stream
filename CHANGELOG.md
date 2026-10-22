# Changelog

## 1.0.0 (2026-10-22)


### ⚠ BREAKING CHANGES

* Normalize repository, dropping Node <26.1.0 ([#151](https://github.com/FotoVerite/gulp-glob-stream/issues/151))
* Switch to streamx ([#119](https://github.com/FotoVerite/gulp-glob-stream/issues/119))
* Combine GlobStream & GlobReadable into unified API
* Replace glob with anymatch & custom directory walk ([#118](https://github.com/FotoVerite/gulp-glob-stream/issues/118))
* Drop support for ordered globs ([#115](https://github.com/FotoVerite/gulp-glob-stream/issues/115))
* Normalize repository, dropping node <10.13 support ([#101](https://github.com/FotoVerite/gulp-glob-stream/issues/101))

### Features

* Combine GlobStream & GlobReadable into unified API ([6aad264](https://github.com/FotoVerite/gulp-glob-stream/commit/6aad264004e4f1a7f1b6e112c5d7e0fc7db72851))
* Replace glob with anymatch & custom directory walk ([#118](https://github.com/FotoVerite/gulp-glob-stream/issues/118)) ([6aad264](https://github.com/FotoVerite/gulp-glob-stream/commit/6aad264004e4f1a7f1b6e112c5d7e0fc7db72851))
* Switch to streamx ([#119](https://github.com/FotoVerite/gulp-glob-stream/issues/119)) ([8d6b35c](https://github.com/FotoVerite/gulp-glob-stream/commit/8d6b35c1f0c89b7869d2ed7ab9e5ec79694e28e2))


### Bug Fixes

* Avoid blowing the call stack when processing many files ([#133](https://github.com/FotoVerite/gulp-glob-stream/issues/133)) ([bb21c9d](https://github.com/FotoVerite/gulp-glob-stream/commit/bb21c9dc14b52ff275e5c4ab3e2c3c7de9dd63f8))
* Avoid following circular symlinks ([#126](https://github.com/FotoVerite/gulp-glob-stream/issues/126)) ([cf8b197](https://github.com/FotoVerite/gulp-glob-stream/commit/cf8b1971a239e165a61654dffeac546faae449fc))
* Avoid joining root paths with cwd ([4344713](https://github.com/FotoVerite/gulp-glob-stream/commit/4344713a37b95ccc903364249511240cdf9a36a5))
* Avoid mutating the options passed in (closes [#75](https://github.com/FotoVerite/gulp-glob-stream/issues/75)) ([f369978](https://github.com/FotoVerite/gulp-glob-stream/commit/f369978f2c861517025d893b4810276f90315fad))
* Avoid pushing additional paths to queue when error occurs ([#124](https://github.com/FotoVerite/gulp-glob-stream/issues/124)) ([8eaab85](https://github.com/FotoVerite/gulp-glob-stream/commit/8eaab85cbc7254d2e74d308c822df50a9e7aaf4a))
* Correctly track found globs against positive globs only ([#150](https://github.com/FotoVerite/gulp-glob-stream/issues/150)) ([2112789](https://github.com/FotoVerite/gulp-glob-stream/commit/2112789b724bf22ff4b11c142b967d6eda439691))
* Do not start and end the stream prematurely ([#136](https://github.com/FotoVerite/gulp-glob-stream/issues/136)) ([9d36482](https://github.com/FotoVerite/gulp-glob-stream/commit/9d364824a925cf10b30ea3cb4f91f7c0cf44784f))
* Ensure basePath is resolved first (fixes gulpjs/gulp[#1744](https://github.com/FotoVerite/gulp-glob-stream/issues/1744)) ([#67](https://github.com/FotoVerite/gulp-glob-stream/issues/67)) ([90c7edb](https://github.com/FotoVerite/gulp-glob-stream/commit/90c7edbd2136e585f2490c92562689ff205222e5))
* Handle Windows path separators when calculating base path on Windows (fixes [#68](https://github.com/FotoVerite/gulp-glob-stream/issues/68)) ([#69](https://github.com/FotoVerite/gulp-glob-stream/issues/69)) ([40128d6](https://github.com/FotoVerite/gulp-glob-stream/commit/40128d6c6343e153eb09bf29a67d58ccc4c57582))
* Ignore directories with invalid permissions ([#146](https://github.com/FotoVerite/gulp-glob-stream/issues/146)) ([003120b](https://github.com/FotoVerite/gulp-glob-stream/commit/003120b450450bd3cd21f164fe8476972cbdd1ab))
* Ignore no-entry errors when reading directories ([#148](https://github.com/FotoVerite/gulp-glob-stream/issues/148)) ([b34ad6d](https://github.com/FotoVerite/gulp-glob-stream/commit/b34ad6d8da2f78318ec2a085c06ba10ca607a9cf))
* Normalize cwd on windows ([8d6b35c](https://github.com/FotoVerite/gulp-glob-stream/commit/8d6b35c1f0c89b7869d2ed7ab9e5ec79694e28e2))
* Normalize path for correct Windows pathing ([7621626](https://github.com/FotoVerite/gulp-glob-stream/commit/7621626fc14404da19a349d777650c6b1ea0e91a))
* Only traverse directories that can match the glob base ([#131](https://github.com/FotoVerite/gulp-glob-stream/issues/131)) ([8e74e21](https://github.com/FotoVerite/gulp-glob-stream/commit/8e74e21840fd38cef4cbce050c99690349b4ee92))
* Pass options to minimatch to handle dotfiles with negative globs (fixes [#18](https://github.com/FotoVerite/gulp-glob-stream/issues/18)) ([3ee8867](https://github.com/FotoVerite/gulp-glob-stream/commit/3ee88679a7a7ea5ab9248d18f8c29d67fa46e5c6))
* Properly handle glob trailing separators with to-absolute-glob (closes [#53](https://github.com/FotoVerite/gulp-glob-stream/issues/53)) ([d4891e7](https://github.com/FotoVerite/gulp-glob-stream/commit/d4891e77885ea08657f7e25864b97ff940379735))
* Properly handle glob-like characters in paths ([#117](https://github.com/FotoVerite/gulp-glob-stream/issues/117)) ([872a957](https://github.com/FotoVerite/gulp-glob-stream/commit/872a957c59cc4d1a1bc674b0370c97809d7c595c))
* Remove relativity on globs & base path to handle glob negation (fixes [#8](https://github.com/FotoVerite/gulp-glob-stream/issues/8)) ([6b9ee25](https://github.com/FotoVerite/gulp-glob-stream/commit/6b9ee2576c42ea4c86d2275993ea87b9d62a11d5))
* Resolve cwd to support relative cwd paths ([8d6b35c](https://github.com/FotoVerite/gulp-glob-stream/commit/8d6b35c1f0c89b7869d2ed7ab9e5ec79694e28e2))
* Resolve globs against root option & avoid passing root option to node-glob (fixes [#37](https://github.com/FotoVerite/gulp-glob-stream/issues/37)) ([55dcf96](https://github.com/FotoVerite/gulp-glob-stream/commit/55dcf96018d5852884da1a915372fa489d220597))
* Revert breaking changes in 4.1.0 release ([bfbd180](https://github.com/FotoVerite/gulp-glob-stream/commit/bfbd180040235e2ae960c96a17b4eb25764fc3a0))
* Switch to combine-stream dependency & filter duplicate paths ([bc1ecde](https://github.com/FotoVerite/gulp-glob-stream/commit/bc1ecde0b973e6b24796ff12e9d8d310589fb69e))
* Traverse symlink folders ([#122](https://github.com/FotoVerite/gulp-glob-stream/issues/122)) ([d49d9bd](https://github.com/FotoVerite/gulp-glob-stream/commit/d49d9bd8042650ce91c190ab0ec20be716b2fade))
* Upgrade glob-parent to fix incorrect base when parens in glob path (closes [#70](https://github.com/FotoVerite/gulp-glob-stream/issues/70)) ([d611fdd](https://github.com/FotoVerite/gulp-glob-stream/commit/d611fdd8368b58234d7e55e6003c7c27b7a35c30))
* Use path.resolve to handle Windows paths properly ([e2a8db8](https://github.com/FotoVerite/gulp-glob-stream/commit/e2a8db845dd1280754173214c8dbb00617d85055))
* Use path.sep instead of '/' for correct Windows pathing ([e618a8d](https://github.com/FotoVerite/gulp-glob-stream/commit/e618a8d464d5613df1252667ce9d9e2c90868417))
* Use stream-combiner to propagate errors ([2d3483c](https://github.com/FotoVerite/gulp-glob-stream/commit/2d3483c1078de4fb6849647c352038aa30542a3e))
* Use strict mode to prevent global leakage ([64acc11](https://github.com/FotoVerite/gulp-glob-stream/commit/64acc110f5fafff19bd5d024ff42fb8ab407d860))
* Use unique-stream to actually remove duplicates (fixes [#9](https://github.com/FotoVerite/gulp-glob-stream/issues/9)) ([009ad12](https://github.com/FotoVerite/gulp-glob-stream/commit/009ad1258d0fdef4e6fcc68d8b9c79263ed1db13))


### Miscellaneous Chores

* Drop support for ordered globs ([#115](https://github.com/FotoVerite/gulp-glob-stream/issues/115)) ([f37bccc](https://github.com/FotoVerite/gulp-glob-stream/commit/f37bccc91cd7ffe5bd61010e10b3a850c134677a))
* Normalize repository, dropping node &lt;10.13 support ([#101](https://github.com/FotoVerite/gulp-glob-stream/issues/101)) ([c110ed1](https://github.com/FotoVerite/gulp-glob-stream/commit/c110ed1602b9bbcb380c97298e9ba41a29a0be40))
* Normalize repository, dropping Node &lt;26.1.0 ([#151](https://github.com/FotoVerite/gulp-glob-stream/issues/151)) ([1d36d1a](https://github.com/FotoVerite/gulp-glob-stream/commit/1d36d1a0330378068f1227ed99773aff01b88dd5))

### [8.0.4](https://www.github.com/gulpjs/glob-stream/compare/v8.0.3...v8.0.4) (2026-10-13)


### Bug Fixes

* Correctly track found globs against positive globs only ([#150](https://www.github.com/gulpjs/glob-stream/issues/150)) ([2112789](https://www.github.com/gulpjs/glob-stream/commit/2112789b724bf22ff4b11c142b967d6eda439691))
* Ignore directories with invalid permissions ([#146](https://www.github.com/gulpjs/glob-stream/issues/146)) ([003120b](https://www.github.com/gulpjs/glob-stream/commit/003120b450450bd3cd21f164fe8476972cbdd1ab))
* Ignore no-entry errors when reading directories ([#148](https://www.github.com/gulpjs/glob-stream/issues/148)) ([b34ad6d](https://www.github.com/gulpjs/glob-stream/commit/b34ad6d8da2f78318ec2a085c06ba10ca607a9cf))

### [8.0.3](https://www.github.com/gulpjs/glob-stream/compare/v8.0.2...v8.0.3) (2025-06-01)


### Bug Fixes

* Do not start and end the stream prematurely ([#136](https://www.github.com/gulpjs/glob-stream/issues/136)) ([9d36482](https://www.github.com/gulpjs/glob-stream/commit/9d364824a925cf10b30ea3cb4f91f7c0cf44784f))

### [8.0.2](https://www.github.com/gulpjs/glob-stream/compare/v8.0.1...v8.0.2) (2024-04-08)


### Bug Fixes

* Avoid blowing the call stack when processing many files ([#133](https://www.github.com/gulpjs/glob-stream/issues/133)) ([bb21c9d](https://www.github.com/gulpjs/glob-stream/commit/bb21c9dc14b52ff275e5c4ab3e2c3c7de9dd63f8))
* Avoid following circular symlinks ([#126](https://www.github.com/gulpjs/glob-stream/issues/126)) ([cf8b197](https://www.github.com/gulpjs/glob-stream/commit/cf8b1971a239e165a61654dffeac546faae449fc))
* Only traverse directories that can match the glob base ([#131](https://www.github.com/gulpjs/glob-stream/issues/131)) ([8e74e21](https://www.github.com/gulpjs/glob-stream/commit/8e74e21840fd38cef4cbce050c99690349b4ee92))

### [8.0.1](https://www.github.com/gulpjs/glob-stream/compare/v8.0.0...v8.0.1) (2024-03-25)


### Bug Fixes

* Avoid pushing additional paths to queue when error occurs ([#124](https://www.github.com/gulpjs/glob-stream/issues/124)) ([8eaab85](https://www.github.com/gulpjs/glob-stream/commit/8eaab85cbc7254d2e74d308c822df50a9e7aaf4a))
* Traverse symlink folders ([#122](https://www.github.com/gulpjs/glob-stream/issues/122)) ([d49d9bd](https://www.github.com/gulpjs/glob-stream/commit/d49d9bd8042650ce91c190ab0ec20be716b2fade))

## [8.0.0](https://www.github.com/gulpjs/glob-stream/compare/v7.0.0...v8.0.0) (2023-04-23)


### ⚠ BREAKING CHANGES

* Switch to streamx (#119)
* Combine GlobStream & GlobReadable into unified API
* Replace glob with anymatch & custom directory walk (#118)
* Drop support for ordered globs (#115)

### Features

* Combine GlobStream & GlobReadable into unified API ([6aad264](https://www.github.com/gulpjs/glob-stream/commit/6aad264004e4f1a7f1b6e112c5d7e0fc7db72851))
* Replace glob with anymatch & custom directory walk ([#118](https://www.github.com/gulpjs/glob-stream/issues/118)) ([6aad264](https://www.github.com/gulpjs/glob-stream/commit/6aad264004e4f1a7f1b6e112c5d7e0fc7db72851))
* Switch to streamx ([#119](https://www.github.com/gulpjs/glob-stream/issues/119)) ([8d6b35c](https://www.github.com/gulpjs/glob-stream/commit/8d6b35c1f0c89b7869d2ed7ab9e5ec79694e28e2))


### Bug Fixes

* Normalize cwd on windows ([8d6b35c](https://www.github.com/gulpjs/glob-stream/commit/8d6b35c1f0c89b7869d2ed7ab9e5ec79694e28e2))
* Properly handle glob-like characters in paths ([#117](https://www.github.com/gulpjs/glob-stream/issues/117)) ([872a957](https://www.github.com/gulpjs/glob-stream/commit/872a957c59cc4d1a1bc674b0370c97809d7c595c))
* Resolve cwd to support relative cwd paths ([8d6b35c](https://www.github.com/gulpjs/glob-stream/commit/8d6b35c1f0c89b7869d2ed7ab9e5ec79694e28e2))


### Miscellaneous Chores

* Drop support for ordered globs ([#115](https://www.github.com/gulpjs/glob-stream/issues/115)) ([f37bccc](https://www.github.com/gulpjs/glob-stream/commit/f37bccc91cd7ffe5bd61010e10b3a850c134677a))

## [7.0.0](https://www.github.com/gulpjs/glob-stream/compare/v6.1.0...v7.0.0) (2021-10-31)


### ⚠ BREAKING CHANGES

* Normalize repository, dropping node <10.13 support (#101)

### Miscellaneous Chores

* Normalize repository, dropping node <10.13 support ([#101](https://www.github.com/gulpjs/glob-stream/issues/101)) ([c110ed1](https://www.github.com/gulpjs/glob-stream/commit/c110ed1602b9bbcb380c97298e9ba41a29a0be40))
