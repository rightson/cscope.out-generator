# cscope.out-generator

**cscope.out-generator** is a simple but powerful tool for generating cscope.out file. 

It supports multiple directories scanning - source code in different location/hierarchy can be included.
It can also convert source path to either relative (default) or absolute path. This feature is useful when including local source code as well as system/3rd-party libraries (or Linux kernel source, for example) is required.

Example usage:

	cd ~/your_local_source_dir
	./cs.sh add .                     # this will scan . directory 
	./cs.sh add ../other_folder1      # this will scan ../other_folder1 directory (relative path)
	./cs.sh *abs* ../other_folder2    # this will scan ../other_folder2 directory and convert to absolute paths
	
Above steps will generate `cscope.out` file separately but the result cscope.out will be the union of the three paths.

All specified paths will be saved to `cscope.list`, and the files located in the specified paths in `cscope.list` will be listed in `cscope.files`.

### Update cscope.out

	./cs.sh update

### Cleanup cscope.out

	./cs.sh clean
	
will remove `cscope.*` files.

### Full Usages

Type ./cs.sh for getting help.
