# If we are the top level Makefile, call the one in the root dir instead
.SILENT:
.PHONY: all
$(filter-out all,$(MAKECMDGOALS)): all
all:
	$(MAKE) -C .. $(patsubst %,library/%,$(or $(MAKECMDGOALS),all))
