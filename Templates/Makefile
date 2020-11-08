#
#
# date : 10/27/2020

TARGET = target

ifndef	CCOMPILER
	CCOMPILER := gcc
endif

#VPATH = include
test = $(pwd)

CC := $(CCOMPILER) 
CFLAGS=-Wall 
INC = -I./include 

src = ./src/main.o 

objects = $(src:.c=.o)
$(TARGET): $(objects)
	$(CC) $(CFLAGS) $(INC)  -o target $(objects)
	echo "$(test)"
%.o: %.c 
	$(CC) $(CFLAGS) $(INC)  -c -o $@ $^




.PHONY:clean
clean: 
	-rm target $(objects)
