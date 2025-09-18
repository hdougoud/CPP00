NAME	= PhoneBook
CC		= c++
FLAGS	= -Wall -Wextra -Werror -std=c++98 -pedantic

SRCS		= Contact.cpp main.cpp PhoneBook.cpp
OBJECT	= $(SRCS:.cpp=.o)

all: $(NAME)
$(NAME) : $(OBJECT)
	$(CC) $(FLAGS) -o $(NAME) $(OBJECT)

%.o: %.c
	$(CC) $(FLAGS) -c $< -o $@

clean:
	rm -rf *.o

fclean: clean
	rm -f $(NAME)

re: fclean all

.PHONY: all clean fclean re