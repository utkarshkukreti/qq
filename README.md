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

## ZSH autocompletion

Add this to your .zshrc (or some script you source from .zshrc)

    # Autocompletion for qq (http://github.com/utkarshkukreti/qq)
    function _qq() {
           _values -S , keys $(qq --keys) && ret=0
    }
    compdef _qq qq

## License

&copy; Utkarsh Kukreti, 2012.

Licensed under the MIT license.
