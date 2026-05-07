# QuadChecker

A Go-based utility for generating and validating quad patterns based on user-specified parameters.

## Overview

QuadChecker is a piscine raid project that provides two core functionalities:

1. **Quad Generation**: Generate ASCII quad patterns based on predefined variants encoded in the source code
2. **Quad Validation**: Verify that user-provided CLI parameters correspond to valid quad configurations

## Prerequisites

- Go 1.16 or higher
- Linux/Unix environment (macOS compatible)

## Installation

Clone the repository and build the quad generators:

```bash
go build -o quadA ./cmd/quadA
go build -o quadB ./cmd/quadB
go build -o quadC ./cmd/quadC
go build -o quadD ./cmd/quadD
go build -o quadE ./cmd/quadE
```

## Usage

To validate a quad configuration, pipe the output of a quad generator to the checker:

```bash
./quadA 3 3 | go run .
```

**Parameters**: 
- First argument: width
- Second argument: height

### Examples

```bash
./quadB 5 4 | go run .
./quadC 2 2 | go run .
```

## Project Structure

- `main.go`: Core validation and CLI logic
- `go.mod`: Go module definition

## License

This project is part of the piscine curriculum.