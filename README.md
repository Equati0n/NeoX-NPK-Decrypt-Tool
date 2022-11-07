# NeoX NPK Decrypt Tool

Tool to decrypt NPK files as they are used in NetEase's NeoX Engine.

## Building

All you have to do to build it is clone it an run on of the following:

```
cargo build --release
```
or to install
```
cargo install --path .
```

## Usage

Example:

```
npktool x script.npk
```

This will extract all the files in script.npk to the `out` directory.

You can also supply a list of .npk files, and if those contain a filelist file, the tool
will automatically detect it and put the files in the original file structure:
> In Eve Echoes the filelist file usually resides in res0.npk
```
npktool x res0.npk res1.npk res2.npk res3.npk res4.npk res5.npk res6.npk res7.npk res8.npk res9.npk res10.npk res11.npk res12.npk
```

More info on how to use it can be found in the help section.
`npktool --help`
