.PHONY: all clean

all: calculator

objects=main.o addition.o subtraction.o multiplication.o division.o

# PATTERN RULES: compiles each of the .c files:
%.o: %.c
	gcc -c $< -o $@

calculator: $(objects)
	gcc $(objects) -o calculator

clean:
	rm -f *.o calculator
	$(MAKE) all
