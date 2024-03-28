## Common Build errors

`command-line option '-m4-nofpu' is not supported by this configuration`
> Run `sed -i 's/-m4-nofpu/-m4a-nofpu/g' Makefile` 


`undefined reference to _stack`
> Add the LD flag `-Wl,--gc-sections`

`unrecognized command line option '--oformat'`
> Remove the extra space before it : `-Wl,--oformat`
