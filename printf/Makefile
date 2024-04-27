CC = gcc
CFLAGS = -Wall -Wextra -Werror
AR = ar rc

NAME = libftprintf.a

SRCS = ft_nb_to_string.c ft_uns_to_string.c ft_strdup.c ft_strlen.c ft_printf.c \
ft_nb_hex.c ft_write_ptr.c ft_write_text.c

OBJECTS = $(SRCS:.c=.o)

all: $(NAME)

$(NAME): $(OBJECTS)
	$(AR) $@ $^

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o  $@

clean:
	rm -f $(OBJECTS)

fclean: clean
	rm -rf $(NAME)

re: fclean all

.PHONY: all clean fclean re