command-template-bash
=====================

Tiny and portable bash script as a executable command

- Script scaffold for command-line tool development
- Features:
  - Command-line argument parser
    - `--debug`: debug mode
    - `--version`: version information
    - `-h, --help`: help message
  - Abort function
  - CPU counter

Usage
-----

1.  Download `command.sh`.

    ```sh
    $ curl -SLO https://raw.githubusercontent.com/dceoy/command-template-bash/master/command.sh
    $ chmod +x command.sh
    ```

2.  Test `command.sh`.

    ```sh
    $ ./command.sh --help
    ```

    Expected output:

    ```
    Tiny and portable bash script as an executable command

    Usage:
      command.sh [--debug] [--cpus=<int>] [--bool] [--var=<str>] [<arg>...]
      command.sh --version
      command.sh -h|--help

    Options:
      --debug           Debug mode
      --cpus=<int>      Limit CPUs for multiprocessing
      --bool            Option without an argument
      --var=<str>       Option with an argument
      --version         Print version
      -h, --help        Print usage

    Arguments:
      <arg>             Main arguments
    ```

3.  Rename and edit the script.

    ```sh
    $ mv command.sh your_command.sh
    $ vim your_command.sh             # => edit
    ```
