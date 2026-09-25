PROGRAMA := programa

# Compilador y flags
CC := gcc
CFLAGS := -Wall -std=c11

# TODO 1: Definir SRCS
SRCS := main.c operaciones.c

# TODO 2: Derivar OBJS a partir de SRCS
OBJS := $(SRCS:.c=.o)

# Regla principal
all: $(PROGRAMA)

# TODO 3: Comando de linkeo
\((PROGRAMA):\)(OBJS)
	\((CC)\)^ -o $(PROGRAMA)

# TODO 4: Regla de patrón para compilar .c -> .o
%.o: %.c
	\((CC)\)(CFLAGS) -c \(< -o\)@

# Regla para limpiar archivos generados
clean:
	rm -f \((PROGRAMA)\)(PROGRAMA).exe $(OBJS)

# TODO 5: Declarar .PHONY
.PHONY: all clean