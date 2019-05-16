command-template-bash
=====================

Tiny and portable bash script as a shell command

- Script scaffold for command-line tool development
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
    $ git clone https://github.com/dceoy/command-template-bash.git
    ```

2.  Copy, rename and edit `command.sh`.

    ```sh
    $ cp command-template-bash/command.sh your_command.sh   # into your command's name
    ```

Default options
---------------

```sh
$ ./command.sh --help
Tiny and portable bash script as a shell command

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
