# solidity-detector-file

A simple CLI tool to detect Solidity files by checking if a given path contains
any `.sol` files.

## Usage

```text
Usage: solidity-detector-file [OPTIONS]

Options:
      --path <PATH>  The path to the file or directory to detect [env: DETECT_PATH=]
  -h, --help         Print help
```

Example:

```bash
solidity-detector-file --path path/to/solidity-file.sol
```

This will output a JSON result:

```json
{
  "pass": true,
  "language": "Solidity"
}
```

## Development

To build this project, you will need to install the following pre-requisites:
[Git](https://git-scm.com/downloads),
[Rust](https://www.rust-lang.org/tools/install) and
[Just](https://github.com/casey/just).

After cloning the repository, you can simply run `just` in the package directory
to list all available commands. For your first local build, please run `just
install` command to install the dependencies for this project.

## Contributing

If anything feels off, or if you feel that some functionality is missing, please
check out the [contributing page](CONTRIBUTING.md). There you will find
instructions for sharing your feedback, building the project locally, and
submitting pull requests to the project.

## License

Copyright (c) The Hummanta Authors. All rights reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
