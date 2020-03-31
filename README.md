# Awesome Go Linters
A curated list of awesome Go linters.

Sponsored by [GolangCI](https://golangci.com): SaaS service for running linters on Github pull requests. Free for Open Source.

<a href="https://golangci.com/"><img src="/go.png" width="250px"></a>

## Contents
* [Cloud Linters](#cloud-linters)
   * [Go Focused](#go-focused)
   * [General Purpose](#general-purpose)
* [Linters](#linters)
   * [Code Formatting](#code-formatting)
   * [Code Complexity](#code-complexity)
   * [Style and Patterns Checking](#style-and-patterns-checking)
   * [Bugs](#bugs)
   * [Unused Code](#unused-code)
   * [Performance](#performance)
   * [Reports](#reports)
   * [Misc](#misc)
* [Linters Helper Tools](#linters-helper-tools)

## Cloud Linters
### Go Focused
* [GolangCI](https://golangci.com/) - Open Source SaaS service for running linters on Github pull requests. Free for Open Source.
* [Golint online](http://go-lint.appspot.com/) - Lints online Go source files on GitHub, Bitbucket and Google Project Hosting using the golint package.
* [GopherCI](https://gopherci.io/) - GopherCI helps you maintain high-quality Go projects, by checking each GitHub Pull Request, for backward incompatible changes, and a suite of other tests.
* [Go Report Card](https://goreportcard.com/) - Go repo report card.

### General Purpose
* [CodeClimate](https://codeclimate.com/) - The open and extensible static analysis platform.
* [CodeFactor](https://www.codefactor.io/) - Automated Code Analysis for repos on GitHub or BitBucket.
* [HoundCI](https://houndci.com/) - Code review tool for GitHub pull requests
* [QuantifiedCode](https://www.quantifiedcode.com/) - Automated code review & repair
* [Scrutinizer](https://scrutinizer-ci.com/) - A proprietery code quality checker that can be integrated with GitHub
* [SideCI](https://sideci.com/) - An automated code reviewing tool. Improving developers' productivity.


## Linters
### Code Formatting
* [dedupimport](https://github.com/nishanths/dedupimport) - Fix duplicate imports that have the same import path but different import names.
* [gofmt](https://golang.org/cmd/gofmt/) - Gofmt formats Go programs. Must have for every project. Don't forget to use -s flag.
* [gofumpt](https://github.com/mvdan/gofumpt) - The tool is a modified fork of gofmt, enforcing a stricter format than gofmt, while being backwards compatible.
* [goimports](https://godoc.org/golang.org/x/tools/cmd/goimports) - Goimports does everything that gofmt does. Additionally it checks unused imports.
* [unindent](https://github.com/mvdan/unindent) - Report code that is unnecessarily indented

### Code Complexity
* [abcgo](https://github.com/droptheplot/abcgo) - ABC metrics for Go source code.
* [depth](https://github.com/360EntSecGroup-Skylar/goreporter/tree/feature-3.0/linters/depth) - Count the maxdepth of go functions. It's helpful to see if a function needs to be splitted into several smaller functions, for readability purpose.
* [funlen](https://github.com/ultraware/funlen) - linter that checks for long functions. It can check both the number of lines and the number of statements.
* [gocyclo](https://github.com/alecthomas/gocyclo) - Computes and checks the cyclomatic complexity of functions.
* [nakedret](https://github.com/alexkohler/nakedret) - nakedret is a Go static analysis tool to find naked returns in functions greater than a specified function length.
* [splint](https://github.com/stathat/splint) - It finds any functions that are too long or have too many parameters or results.

### Style and Patterns Checking
* [dogsled](https://github.com/alexkohler/dogsled) - Finds assignments/declarations with too many blank identifiers.
* [dupl](https://github.com/mibk/dupl) - Tool for code clone detection.
* [go-checkstyle](https://github.com/qiniu/checkstyle) - checkstyle is a style check tool like java checkstyle. This tool inspired by java checkstyle, golint. The style refered to some points in Go Code Review Comments.
* [go-cleanarch](https://github.com/roblaszczak/go-cleanarch) - go-cleanarch was created to validate Clean Architecture rules, like a The Dependency Rule and interaction between packages in your Go projects.
* [go-consistent](https://github.com/Quasilyte/go-consistent) - source code analyzer that helps you to make your Go programs more consistent.
* [go-namecheck](https://github.com/Quasilyte/go-namecheck) - source code analyzer that helps you to maintain variable/field naming conventions inside your project.
* [go-printf-func-name](https://github.com/jirfag/go-printf-func-name) - checks that printf-like functions are named with `f` at the end.
* [go-ruleguard](https://github.com/quasilyte/go-ruleguard) - Define and run pattern-based custom linting rules.
* [gochecknoinits](https://4d63.com/gochecknoinits) - Find init functions, to reduce side effects in code.
* [gochecknoglobals](https://4d63.com/gochecknoglobals) - Find global vars, to reduce side effects in code.
* [goconst](https://github.com/jgautheron/goconst) - Find in Go repeated strings that could be replaced by a constant.
* [GoLint](https://github.com/golang/lint) - Golint is a linter for Go source code.
* [gosimple](https://github.com/dominikh/go-tools/tree/master/cmd/gosimple) - gosimple is a linter for Go source code that specialises on simplifying code.
* [impi](https://github.com/pavius/impi) - Verify imports grouping and ordering.
* [interfacer](https://github.com/mvdan/interfacer) - Linter that suggests narrower interface types.
* [lll](https://github.com/walle/lll) - Line length linter, used to enforce line length in files.
* [misspell](https://github.com/client9/misspell) - Finds commonly misspelled English words
* [nofuncflags](https://github.com/fsamin/nofuncflags) - disallow boolean params to functions (flags).
* [predeclared](https://github.com/nishanths/predeclared) - Find code that shadows Go's built-in identifiers (e.g., `append`, `copy`, `int`).
* [revive](https://github.com/mgechev/revive) - ~6x faster, stricter, configurable, extensible, and beautiful drop-in replacement for golint
* [unconvert](https://github.com/mdempsky/unconvert) - Remove unnecessary type conversions from Go source.
* [usedexports](https://github.com/jgautheron/usedexports) - Find in Go exported variables that could be unexported.
* [whitespace](https://github.com/ultraware/whitespace) - Checks for unnecessary newlines at the start and end of functions

### Bugs
* [apicompat](https://github.com/bradleyfalzon/apicompat) - Checks recent changes to a Go project for backwards incompatible changes.
* [badtime](https://github.com/m3db/build-tools/tree/master/linters/badtime) - Badtime is a Golang linter that detects inappropriate usage of the time.Time struct.
* [bodyclose](https://github.com/timakin/bodyclose) -  checks whether HTTP response body is closed and a re-use of TCP connection is not blocked
* [durcheck](https://github.com/hypnoglow/durcheck) - durcheck is a very simple linter which detects potential bugs with time.Duration in a Go package.
* [enumcase](https://github.com/MakeNowJust/enumcase) - enumcase checks every switch statement handles all const values of the type.
* [enumlinter](https://github.com/THE108/enumlinter) - Enum linter for enumerated types in Go.
* [errcheck](https://github.com/kisielk/errcheck) - Errcheck is a program for checking for unchecked errors in Go programs.
* [gas](https://github.com/GoASTScanner/gas) - Inspects source code for security problems by scanning the Go AST.
* [go vet](https://golang.org/cmd/vet/) - Vet examines Go source code and reports suspicious constructs, such as Printf calls whose arguments do not align with the format string. Can check shadowing of variables, but must be enabled explicitly.
* [gosumcheck](https://github.com/haya14busa/gosum) - Checks all possible cases of type-switch are handled.
* [go-sumtype](https://github.com/BurntSushi/go-sumtype) - Checks all possible cases of type-switch are handled.
* [mulint](https://github.com/gnieto/mulint) - Go lint which detects recursive locks, which may lead to dead locks.
* [safesql](https://github.com/stripe/safesql) - Static analysis tool for Golang that protects against SQL injections.
* [scopelint](https://github.com/kyoh86/scopelint) - scopelint checks for unpinned variables in go programs.
* [sqlrows](https://github.com/gostaticanalysis/sqlrows) - checks whether Close on sql.Rows is called.
* [staticcheck](https://github.com/dominikh/go-tools/tree/master/cmd/staticcheck) - staticcheck is `go vet` on steroids, applying a ton of static analysis checks you might be used to from tools like ReSharper for C#.

### Unused Code
* [deadcode](https://github.com/tsenart/deadcode) - Finds unused code.
* [ineffassign](https://github.com/gordonklaus/ineffassign) - Detect when assignments to existing variables are not used.
* [structcheck](https://github.com/opennota/check) - Find unused global variables and constants.
* [unparam](https://github.com/mvdan/unparam) - Report unused function parameters.
* [unused](https://github.com/dominikh/go-tools/tree/master/cmd/unused) - unused checks Go code for unused constants, variables, functions and types.
* [varcheck](https://gitlab.com/opennota/check) - Find unused global variables and constants.

### Performance
* [aligncheck](https://github.com/opennota/check) - Warn about un-optimally aligned structures.
* [Copyfighter](https://github.com/jmhodges/copyfighter) - Statically analyzes Go code and reports functions that are passing large structs by value.
* [maligned](https://github.com/mdempsky/maligned) - Tool to detect Go structs that would take less memory if their fields were sorted.
* [prealloc](https://github.com/alexkohler/prealloc) - Find slice declarations that could potentially be preallocated.
* [rangerdanger](https://github.com/mdempsky/rangerdanger) - Tool to detect range statements iterating over addressable arrays

### Reports
* [flen](https://github.com/lafolle/flen) - Get info on length of functions in a Go package.
* [GoReporter](https://github.com/360EntSecGroup-Skylar/goreporter) - A Golang tool that does static analysis, unit testing, code review and generate code quality report.
* [golinters](https://github.com/thomasheller/golinters) - golinters generates HTML reports about Go linters.

### Misc
* [go-outdated](https://github.com/firstrow/go-outdated) - Console application that displays outdated packages.
* [go-template-lint](https://github.com/sourcegraph/go-template-lint) - go-template-lint is a linter for Go text/template (and html/template) template files.
* [godox](https://github.com/766b/godox) - Find all TODO/FIXME comments.
* [lingo](https://github.com/s2gatev/lingo) - Set of specific checks.
* [megacheck](https://github.com/dominikh/go-tools/tree/master/cmd/megacheck) - megacheck runs staticcheck, gosimple and unused at once. Because it is able to reuse work, it will be faster than running each tool separately.
* [go-critic](https://github.com/go-critic/go-critic) - source code linter that brings checks that are currently not implemented in other linters.
* [tarp](https://github.com/verygoodsoftwarenotvirus/tarp) - tarp finds functions and methods without direct unit tests in Go source code.
* [go-mnd](https://github.com/tommy-muehle/go-mnd) - Magic number detector for Go.
* [gocheckit](https://github.com/brompwnie/gocheckit) - A Go tool to help identify Deprecated Go Modules.

## Linters Helper Tools
* [golangci-lint](https://github.com/golangci/golangci-lint) - Linters Runner for Go. 5x faster than gometalinter. Nice colored output. Can report only new issues. Fewer false-positives. Yaml/toml config.
* [gometalinter](https://github.com/alecthomas/gometalinter) - Metalinter is a tool to automatically apply all static analysis tool and report their output in normalized form.
* [lint](https://github.com/surullabs/lint) - Run linters as part of go test.
* [revgrep](https://github.com/bradleyfalzon/revgrep) - Filters output from static analysis tools, showing only recently changed lines of code
* [reviewdog](https://github.com/haya14busa/reviewdog) - "reviewdog" provides a way to post review comments to code hosting service, such as GitHub, automatically by integrating with any linter tools with ease.
* [zb](https://github.com/joshuarubin/zb) - speedup linting by caching gometalinter result.
