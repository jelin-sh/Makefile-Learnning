.PHONY:clean

CC = gcc
RM = rm

TARGET = HelloWorld
SOURCE = foo.c main.c func.c
OBJECTS = ${SOURCE:.c=.o}

${TARGET}: ${OBJECTS}
	${CC} -o $@ $^ 
%.o: %.c
	${CC} -o $@ -c $^

clean:
	@echo "clear output"
	@${RM} ${OBJECTS}
	@echo "ok"
