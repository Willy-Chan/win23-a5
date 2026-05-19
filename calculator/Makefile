.PHONY: all clean

all: calculator

objects=main.o addition.o subtraction.o multiplication.o division.o

# PATTERN RULES: compiles each of the .c files:
%.o: %.c
	clang -c $< -o $@

calculator: $(objects)
	clang $(objects) -o calculator

clean:
	rm -f *.o calculator
	$(MAKE) all
