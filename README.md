# hashname

hashname is a python script to rename files by their hash, preserving file types, to avoid collisions.
The reason it was created was dumping files from cameras and scanners where there is an incrementing numeric suffix on each image.

## Usage
    hashname <files>

Options:

Short | Long | Description
--- | --- | ---
`-h` | `--help` | Prints help, terminates after printing
`-q` | `--quiet` | Does not print status information
`-s` | `--safe` | Will not delete duplicated files
`-c` | `--caps` | Makes each extention lowercase
`-j` | `--jpg` | Sets all `jpeg` extentions to `jpg`

After `--` is treated as a file, not an argument.

Hash function options:

*  `--md5`
*  `--sha1` (default)
*  `--sha224`
*  `--sha256`
*  `--sha384`
*  `--sha512`

Every hash function that is garanteed support in every interpreter is an option.
