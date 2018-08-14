# Go
Scaffolding for medium-sized Go projects with Dep integration.

## Directory Setup
The project scaffold has the following structure:
/project-dir
	/cmd (code for binaries built with program)
		/first (will install as "first")
			first.go
		/second (will install as "second")
			second.go
	/build (build artifacts)
	/bin (installed binaries)
		first (generated by make build)
		second ...
	/pkg1 (standard go package)
	/pkg2 ...
	/pgk3 ...

## Standard workflow
1. edit code
2. `make ensure` (ensures dependencies)
3. `make test` (runs all tests)
4. `make bench` (runs all benchmarks)
5. `make build` (builds binaries)
6. use binaries!