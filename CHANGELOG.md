# Change Log

## [1.3.0](https://github.com/grammarly/rocker/tree/1.3.0)

[Full Changelog](https://github.com/grammarly/rocker/compare/1.2.0...1.3.0)

**Merged pull requests:**

- Refactor commands to use composition [\#128](https://github.com/grammarly/rocker/pull/128) ([ybogdanov](https://github.com/ybogdanov))
- Implement ARG command and --build-arg flag [\#126](https://github.com/grammarly/rocker/pull/126) ([ybogdanov](https://github.com/ybogdanov))
- Support different regions for AWS ECR, fixes \#105 [\#124](https://github.com/grammarly/rocker/pull/124) ([ybogdanov](https://github.com/ybogdanov))
- Rocker to print command if env variable is present [\#123](https://github.com/grammarly/rocker/pull/123) ([ybogdanov](https://github.com/ybogdanov))
- Refactor integration tests, so they run on TravisCI [\#122](https://github.com/grammarly/rocker/pull/122) ([ybogdanov](https://github.com/ybogdanov))
- Fix mount loop processing to avoid crash on invalid path [\#121](https://github.com/grammarly/rocker/pull/121) ([aacebedo](https://github.com/aacebedo))
- Docker 1.12 compatibility, make integration tests run under Docker for Mac [\#118](https://github.com/grammarly/rocker/pull/118) ([ybogdanov](https://github.com/ybogdanov))
- Warn about implicit contextDir change [\#117](https://github.com/grammarly/rocker/pull/117) ([ctrlok](https://github.com/ctrlok))
- Rockerfile.tmLanguage: highlight `LABEL` [\#107](https://github.com/grammarly/rocker/pull/107) ([igrayson](https://github.com/igrayson))

## [1.2.0](https://github.com/grammarly/rocker/tree/1.2.0)

[Full Changelog](https://github.com/grammarly/rocker/compare/1.1.2...1.2.0)

**Merged pull requests:**

- Calculate image size difference using parent image size [\#100](https://github.com/grammarly/rocker/pull/100) ([diunko](https://github.com/diunko))
- Enable PATH variable to be expanded as default value, if not set by prior ENV command [\#98](https://github.com/grammarly/rocker/pull/98) ([diunko](https://github.com/diunko))
- Remove go-vet dependency for tests, it is already in golang [\#95](https://github.com/grammarly/rocker/pull/95) ([ybogdanov](https://github.com/ybogdanov))
- Better error message if context dir arg is not a directory  [\#93](https://github.com/grammarly/rocker/pull/93) ([ctrlok](https://github.com/ctrlok))
- Support urls as ADD sources [\#91](https://github.com/grammarly/rocker/pull/91) ([diunko](https://github.com/diunko))
- Expand variables at the time of ONBUILD command execution [\#90](https://github.com/grammarly/rocker/pull/90) ([diunko](https://github.com/diunko))
- Better mount error [\#87](https://github.com/grammarly/rocker/pull/87) ([romank87](https://github.com/romank87))
- Update go-dockerclient [\#86](https://github.com/grammarly/rocker/pull/86) ([romank87](https://github.com/romank87))
- Rewrite export/import cache logic [\#85](https://github.com/grammarly/rocker/pull/85) ([romank87](https://github.com/romank87))
- Fix mount in matrix [\#79](https://github.com/grammarly/rocker/pull/79) ([romank87](https://github.com/romank87))
- Integration tests [\#78](https://github.com/grammarly/rocker/pull/78) ([romank87](https://github.com/romank87))

## [1.1.2](https://github.com/grammarly/rocker/tree/1.1.2)

[Full Changelog](https://github.com/grammarly/rocker/compare/1.1.1...1.1.2)

**Merged pull requests:**

- New S3 naming schema works in parallel to the old one [\#76](https://github.com/grammarly/rocker/pull/76) ([romank87](https://github.com/romank87))
- Adopt S3 naming schema for Docker v1.10 [\#75](https://github.com/grammarly/rocker/pull/75) ([romank87](https://github.com/romank87))

## [1.1.1](https://github.com/grammarly/rocker/tree/1.1.1)

[Full Changelog](https://github.com/grammarly/rocker/compare/1.1.0...1.1.1)

**Merged pull requests:**

- Use git branch names as tags for docker images [\#70](https://github.com/grammarly/rocker/pull/70) ([romank87](https://github.com/romank87))

## [1.1.0](https://github.com/grammarly/rocker/tree/1.1.0) (2016-01-29)
[Full Changelog](https://github.com/grammarly/rocker/compare/1.0.1...1.1.0)

**Implemented enhancements:**

- Use GO15VENDOREXPERIMENT, get rid of gb, restructure the project layout [\#67](https://github.com/grammarly/rocker/issues/67)
- Configurable push retries [\#66](https://github.com/grammarly/rocker/issues/66)
- Print rocker version when -cmd \(-C\) flag specified [\#64](https://github.com/grammarly/rocker/issues/64)
- Support credentials stored by "docker login" for authentication [\#57](https://github.com/grammarly/rocker/issues/57)
- Ability to directly PUSH and PULL from S3, without using Registry [\#53](https://github.com/grammarly/rocker/issues/53)
- Do not wrap proxied output from containers with logger [\#47](https://github.com/grammarly/rocker/issues/47)
- Configurable push retries [\#62](https://github.com/grammarly/rocker/pull/62) ([ybogdanov](https://github.com/ybogdanov))

**Fixed bugs:**

- Some kind of error stack trace [\#49](https://github.com/grammarly/rocker/issues/49)
- COPY/ADD does not copy symlinks [\#60](https://github.com/grammarly/rocker/issues/60)
- "bufio.Scanner: token too long" while passing output from a container [\#54](https://github.com/grammarly/rocker/issues/54)
- Cannot ^C while pulling an image [\#16](https://github.com/grammarly/rocker/issues/16)
- Exit with non-zero code when get unexpected EOF on PUSH [\#52](https://github.com/grammarly/rocker/pull/52) ([ctrlok](https://github.com/ctrlok))

## [1.0.1](https://github.com/grammarly/rocker/tree/1.0.1) (2015-11-26)
[Full Changelog](https://github.com/grammarly/rocker/compare/1.0.0...1.0.1)

**Fixed bugs:**

- EXPORT/IMPORT is not working with Docker 1.9: rsync-static container volumes [\#51](https://github.com/grammarly/rocker/issues/51)

## [1.0.0](https://github.com/grammarly/rocker/tree/1.0.0) (2015-11-23)
[Full Changelog](https://github.com/grammarly/rocker/compare/0.2.3...1.0.0)

**Implemented enhancements:**

- Ability to lookup images by fuzzy semver tags [\#46](https://github.com/grammarly/rocker/issues/46)
- rocker/template: `image` helper that can read artifacts [\#45](https://github.com/grammarly/rocker/issues/45)
- Export artifacts as a build result [\#44](https://github.com/grammarly/rocker/issues/44)
- do not create .rockerignore for user [\#27](https://github.com/grammarly/rocker/issues/27)
- Read Rockerfile from STDIN [\#15](https://github.com/grammarly/rocker/issues/15)
- Rewrite MOUNT and $GIT\_SSH\_KEY readme due to the new template engine [\#14](https://github.com/grammarly/rocker/issues/14)
- making rocker requires rocker [\#1](https://github.com/grammarly/rocker/issues/1)
- V1 - rewrite Rocker from scratch, completely client-driven [\#50](https://github.com/grammarly/rocker/pull/50) ([ybogdanov](https://github.com/ybogdanov))

**Fixed bugs:**

- v1: "COPY a\*.js ./" is not working properly [\#48](https://github.com/grammarly/rocker/issues/48)
- Ability to update $PATH env variable \(compatibility with docker\) [\#42](https://github.com/grammarly/rocker/issues/42)
- WARN\[0000\] Tar: Can't archive a file with includes [\#40](https://github.com/grammarly/rocker/issues/40)
- Make in the rocker's Rockerfile does not work with Go 1.5  [\#26](https://github.com/grammarly/rocker/issues/26)

## [0.2.3](https://github.com/grammarly/rocker/tree/0.2.3) (2015-11-23)
[Full Changelog](https://github.com/grammarly/rocker/compare/0.2.2...0.2.3)

**Implemented enhancements:**

- Would be nice to get results of `rocker show` in creation time order [\#25](https://github.com/grammarly/rocker/issues/25)
- \[experiment\] make rocker create a light semver aliases for published tags [\#9](https://github.com/grammarly/rocker/issues/9)
- rocker/template: include [\#37](https://github.com/grammarly/rocker/issues/37)
- Store information about pushed images as artifact files [\#35](https://github.com/grammarly/rocker/issues/35)
- rocker/template: load vars from file [\#34](https://github.com/grammarly/rocker/issues/34)
- rocker/template: call strings helper "indexOf" instead of "index" [\#33](https://github.com/grammarly/rocker/issues/33)
- Hightlight INCLUDE for sublime text language [\#29](https://github.com/grammarly/rocker/issues/29)
- rocker/template: other template string helpers [\#22](https://github.com/grammarly/rocker/issues/22)
- rocker/template: shell helper [\#20](https://github.com/grammarly/rocker/issues/20)
- rocker/template: yaml helper [\#19](https://github.com/grammarly/rocker/issues/19)
- rocker/template: json helper [\#18](https://github.com/grammarly/rocker/issues/18)
- Do not fail on gathering git info, give a warning instead [\#17](https://github.com/grammarly/rocker/issues/17)
- rocker/template: load variable content from a file [\#13](https://github.com/grammarly/rocker/issues/13)

**Fixed bugs:**

- Randomly appearing IMPORT/EXPORT problem in rocker [\#8](https://github.com/grammarly/rocker/issues/8)
- Image fails to parse if registry is an ip with a port [\#24](https://github.com/grammarly/rocker/issues/24)
- Adopt image name splitting logic from docker [\#41](https://github.com/grammarly/rocker/pull/41) ([fxposter](https://github.com/fxposter))

**Merged pull requests:**

- Fix Windows inability to handle a tilde as the home directory [\#43](https://github.com/grammarly/rocker/pull/43) ([tyrken](https://github.com/tyrken))
- ability to create artifacts without push images to regestry [\#36](https://github.com/grammarly/rocker/pull/36) ([ctrlok](https://github.com/ctrlok))
- \#22 integrate Go's string functions to the template [\#23](https://github.com/grammarly/rocker/pull/23) ([ybogdanov](https://github.com/ybogdanov))
- Merge template functions collected in Dev branch [\#21](https://github.com/grammarly/rocker/pull/21) ([ybogdanov](https://github.com/ybogdanov))

## [0.2.2](https://github.com/grammarly/rocker/tree/0.2.2) (2015-09-17)
[Full Changelog](https://github.com/grammarly/rocker/compare/0.2.1...0.2.2)

**Fixed bugs:**

- ATTACH does not restore the terminal from the raw mode when finished [\#11](https://github.com/grammarly/rocker/issues/11)

**Closed issues:**

- `default` templating function is not present in rocker but present in rocker-compose [\#12](https://github.com/grammarly/rocker/issues/12)
- Add `id` parameter to rocker to override default Rockerfile cache key [\#6](https://github.com/grammarly/rocker/issues/6)

**Merged pull requests:**

- implements \#9 [\#10](https://github.com/grammarly/rocker/pull/10) ([ybogdanov](https://github.com/ybogdanov))

## [0.2.1](https://github.com/grammarly/rocker/tree/0.2.1) (2015-09-14)
[Full Changelog](https://github.com/grammarly/rocker/compare/0.2.0...0.2.1)

**Implemented enhancements:**

- MOUNT is not respecting ~ alias [\#4](https://github.com/grammarly/rocker/issues/4)

**Merged pull requests:**

- \#6 provide `-id` parameter [\#7](https://github.com/grammarly/rocker/pull/7) ([ybogdanov](https://github.com/ybogdanov))
- Issue 4 [\#5](https://github.com/grammarly/rocker/pull/5) ([ybogdanov](https://github.com/ybogdanov))

## [0.2.0](https://github.com/grammarly/rocker/tree/0.2.0) (2015-09-08)


\* *This Change Log was automatically generated by [github_changelog_generator](https://github.com/skywinder/Github-Changelog-Generator)*


\* *This Change Log was automatically generated by [github_changelog_generator](https://github.com/skywinder/Github-Changelog-Generator)*


\* *This Change Log was automatically generated by [github_changelog_generator](https://github.com/skywinder/Github-Changelog-Generator)*


\* *This Change Log was automatically generated by [github_changelog_generator](https://github.com/skywinder/Github-Changelog-Generator)*
