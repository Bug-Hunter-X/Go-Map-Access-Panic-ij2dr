# Go Map Access Panic

This repository demonstrates a common error in Go: accessing a map element without checking if the map is nil.  This can lead to a runtime panic.

## Bug

The `bug.go` file contains code that attempts to access a map element without checking if the map is initialized.  If the map is nil, this will result in a panic.

## Solution

The `bugSolution.go` file provides a corrected version of the code. It checks if the map is nil before accessing an element, preventing the panic.

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `go run bug.go` to see the panic.
4. Run `go run bugSolution.go` to see the corrected behavior.