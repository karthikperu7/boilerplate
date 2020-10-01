This is a dummy project used to test the `generate-check` make target for go operator (like in `openshift/golang-osd-operator`).

#### Projects main points
- This is an operator initialized with `operator-sdk v0.16` in order to have all the `make generate` commands working properly
- The `go.mod` file have been templatized to allow testing of several versions of `operator-sdk` with the same base project (actual `go.mod` is generated by a sed command on the template)
- There are 2 dummy files (`src/test/test.go` and `src/test/subfolder/test.go`) containing basic generate commands which are tested/validated in the test case