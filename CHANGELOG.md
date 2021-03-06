# Change log

This log documents significant changes for each release.  This project follows
[Semantic Versioning](http://semver.org/).

## [0.9.0] - 2018-10-27
### Added
 - Support for environment variables

## [0.8.2] - 2018-10-24
### Fixed
 - Issues with decimals and the ~ operator.

## [0.8.1] - 2018-10-10
### Fixed
 - Floating point arithemetic errors are now corrected prior to comparison.

## [0.8.0] - 2018-09-21
### Added
 - Support for "contains" and "in" operators
 - Support for parentheses and null literals

## [0.7.0] - 2018-09-19
### Added
 - An option to the demo app for working with JSON rather than YAML.

## [0.6.0] - 2018-09-07
### Added
 - logical operations
 - tree navigation
 - string functions
 - part of ofType (explicit one)

## [0.5.1] - 2018-09-07
### Fixed
 - Corrected the (outdated) main file entry in package.json.

## [0.5.0] - 2018-09-07
### Added
 - combine()
### Fixed
 - union operator ("|")

## [0.4.3] - 2018-09-05
### Fixed
 - A problem with subsetOf (and supersetOf) that prevented objects with keys
   added in different orders from being considered the same.

## [0.4.1] - 2018-08-29
### Added
 - Tests for functions in 5.2 (except ofType), which is not yet implemented.

## [0.4.0] - 2018-08-27
### Added
 - Remaining functions in 5.1 (Existence) of the FHIRPath specification.

## [0.3.0] - 2018-08-24
### Added
 - Support for $this
 - all/any True/False.
 - Support for !~ and  =~

## [0.2.3] - 2018-08-13
### Changed
 - Reorgnanized math functions into a separate file.

## [0.2.2] - 2018-08-10
### Changed
 - Revised internal routines so everything is handled as a collection.

## [0.2.1] - 2018-08-07
### Fixed
 - An unexpected (math) operator error that happened when the code was
   minimized.

## [0.2.0] - 2018-08-07
### Added
 - Handles all math operations defined in 6.6 of the FHIRPath specification.
 - take, last, tail
 - iif
### Fixed
 - skip

## [0.1.1] - 2018-08-02
### Added
 - GitHub repository to package.json.

## [0.1.0] - 2018-08-01
### Added
 - Added beginning of a FHIRPath engine.  There is name a script bin/fhirpath
   which will take a FHIRPath expression and a filename containing a JSON FHIR
   resource, and prints the result of the expression (for many basic
   expressions).  Without the filename, it prints the parsed expression tree,
   which is what bin/parseAndDisplay.js used to do, so that has been removed.

## [0.0.1] - 2018-07-23
### Added
 - There is a now a parser and a small script (bin/parseAndDisplay.js) which
   prints out the parse tree of a FHIRPath expression.

