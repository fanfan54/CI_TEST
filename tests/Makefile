##
## EPITECH PROJECT, 2017
## Makefile for Day10
## File description:
## Even if I'm not tested on this one
##

SRC		=	tests.c 		\
			../src/fibo.c

H_DIR	=	../include

CPPFLAGS=	-I $(H_DIR)

OBJ		=	$(SRC:.c=.o)

NAME	=	tests

CFLAGS	=	-lcriterion

all:	$(NAME)

$(NAME):	$(OBJ)
	#@echo -e "\e[34mWe are compiling objects\e[39m"
	#gcc -c $(SRC) -Wall -Wextra -Werror --pedantic
	@echo -e "\e[34mWe are linking the objects into a lib\e[39m"
	$(CC) $(CFLAGS) -o $(NAME) $(OBJ)

clean:
	@echo -e "\e[34mRemoving objects files\e[39m"
	rm -f $(OBJ)


fclean:	clean
	@echo -e "\e[34mDeleting the compiled bin\e[39m"
	rm -f $(NAME)

re:	fclean all

.PHONY: all clean fclean re tests_run
