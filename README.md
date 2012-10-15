# qq

A simple utility to store and access key/value pairs from the shell, useful for storing common urls, etc.

The database is stored in a yaml file in `~/.qq`

## Installation

    git clone https://github.com/utkarshkukreti/qq.git
    cd qq
    ln -s "$(pwd)/qq" /usr/local/bin

## Usage

    List
      qq
    Add:
      qq <key> <value>
    Fetch
      qq <key>
    Help
      qq --help

## License

&copy; Utkarsh Kukreti, 2012.

Licensed under the MIT license.
