# pads
pads is a utility that allows you to manage alternate data streams stored in the NTFS file system.

# Usage:
pads [options] inputfile

# Options:

    -l path,  --list=path
        List alternate data streams attached to file or directory.
        Example: pads [-v] -l inputfile

    -d path,  --list-dir=path
        List alternate data streams attached to files in directory.
        Use -r flag for recursive mode.
        Example: pads [-r] [-v] -d [path]

    -x stream,  --extract=stream
        Extract alternate data stream from file or directory.
        Example: pads [-n filename] -x streamname inputfile

    -a path,  --add=path
        Add alternate data stream to file or directory.
        Example: pads [-n filename] -a streamfile inputfile

    -n name,  --file-name=name
        Provide new name for file or stream.

    -o path,  --output=path
        Provide output file name.

    -p path,  --pack=path
        Pack file or folder and add as stream.
        Example: pads [-v] [-n streamname] -p in_path inputfile

    -u,  --unpack
        Unpack and extract stream.
        Example: pads [-v] [-n streamname] [-o out_path] -u inputfile

    --list-packed
        List packed stream.
        Example: pads [-v] [-n streamname] --list-packed inputfile

    -r,  --recursive
        Recursive mode.

    -v,  --verbose
        Detailed mode.

    --remove=name
        Remove alternate data stream.
        Example: pads --remove=streamname inputfile

    -h,  --help
        Print this message and exit.

    -V,  --version
        Display version information and exit.
