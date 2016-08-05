# html prettyprinter (FORKED)

[![Known Vulnerabilities](https://snyk.io/test/github/apiaryio/commonjs-html-prettyprinter/badge.svg)](https://snyk.io/test/github/apiaryio/commonjs-html-prettyprinter)

Fork of [commonjs-html-prettyprinter](https://github.com/maxogden/commonjs-html-prettyprinter). The reason for forking the project is [this security issue](https://snyk.io/vuln/npm:minimatch:20160620). [Dredd](https://github.com/apiaryio/dredd) temporarily depends on this fork until the security issue gets resolved.

## Fix

[maxogden/commonjs-html-prettyprinter#12](https://github.com/maxogden/commonjs-html-prettyprinter/pull/12) aims to resolve the issue in upstream. Once it's merged and new version of the project published to npm, this fork should get deprecated.

## How the Fork Works

- There's branch `honzajavorek/upgrade-glob` with fix and PR [maxogden/commonjs-html-prettyprinter#12](https://github.com/maxogden/commonjs-html-prettyprinter/pull/12) made from that branch.
- The `master` branch of this repository cherry-picks the commit with fix and adds more (README update).
- Since [apiaryio/dredd#589](https://github.com/apiaryio/dredd/pull/589) PR, [Dredd](https://github.com/apiaryio/dredd) depends on the is in the `honzajavorek/upgrade-glob` branch of this fork.
