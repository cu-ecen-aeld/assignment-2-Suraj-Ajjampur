COMPILER ?= $(CROSS_COMPILER)gcc

#Flags to treat all the warnings as errors
FLAGS=-Wall -Werror

# writer recipe

.PHONY : all
all: writer

#Linking all the compiled object files
writer: writer_o
	$(COMPILER) $(FLAGS) writer.o -o writer

# Compiling the source files to generate object files
writer_o:
	$(COMPILER) $(FLAGS) -c writer.c -o writer.o

# Clean the working directory
.PHONY: clean
clean:
	rm -f *.o writer
#
