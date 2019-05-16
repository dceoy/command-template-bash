bash-command-template
=====================

Template bash script for command-line tool development

- Tiny and portable script as an executable command
- Features:
  - Command-line argument parser
    - `--debug`: debug mode
    - `--help`: help message
    - `--version`: version information
  - Abort function
  - CPU counter

Usage
-----

1.  Check out the repository.

    ```sh
    $ git clone https://github.com/dceoy/bash-command-template.git
    ```

2.  Copy, rename and edit `command.sh`.

    ```sh
    $ cp bash-command-template/command.sh your_command.sh   # into your command's name
    ```

Default options
---------------

```sh
$ ./command.sh --help
Template bash script for command-line tool development

Usage:
  command.sh [--debug] [--cpus=<int>] [--bool] [--var=<str>] [<arg>...]
  command.sh -h|--help
  command.sh --version

Options:
  --debug           Debug mode
  --cpus=<int>      Limit CPUs for multiprocessing
  --bool            Option without an argument
  --var=<str>       Option with an argument
  -h, --help        Print usage
  --version         Print version

Arguments:
  <arg>             Main arguments
```
