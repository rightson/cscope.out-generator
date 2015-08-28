# cscope.out-generator

cscope.out-generator is a script for generating cscope.out file.
it can specify multiple directories (it support both relative and absolute path)

Example usage:

	cd ~/your_driver_source_dir
	./cs.sh add .                     # this will scan . directory 
	./cs.sh add ../other_folder1      # this will scan ../other_folder1 directory (relative path)
	./cs.sh abs ../other_folder2      # this will scan ../other_folder2 directory and convert to absolute paths
	
above steps will generate `cscope.out` file separately but the result cscope.out will be the union of the three paths.

Type ./cs.sh for getting help.
