.PHONY: resolve validate jobs-tests

resolve:
	dep ensure -v -vendor-only

validate: resolve
	./before-commit.sh

jobs-tests: resolve
	go test -v ./jobs/...