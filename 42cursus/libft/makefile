LIB = ar rcs
NAME = libft.a

CC = gcc

CCFLAGS =-Wall -Wextra -Werror

RM = rm -rf

SRC = ft_alpha.c ft_isdigit.c ft_isalnum.c ft_isascii.c ft_isprint.c ft_strlen.c ft_memset.c ft_bzero.c ft_memcpy.c ft_memmove.c ft_strlcpy.c ft_strlcat.c ft_toupper.c ft_tolower.c ft_strchr.c ft_strrchr.c ft_strncmp.c ft_memchr.c ft_memcmp.c ft_strnstr.c ft_atoi.c ft_calloc.c ft_substr.c ft_strjoin.c ft_strtrim.c ft_split.c ft_itoa.c ft_strmapi.c ft_striteri.c ft_putchar_fd.c ft_putstr_fd.c ft_putendl_fd.c ft_putnbr_fd.c

OBJ = $(SRC:%.c=%.o)
INCLUDE = libft.h

$(NAME) : $(OBJ) $(INCLUDE)
	$(LIB) $(NAME) $(OBJ)

all : $(NAME)

%.o : %.c
	@$(CC) $(CCFLAGS) -c -o $@ $<
clean:
	@$(RM) $(OBJ)
fclean: clean
	@rm -f $(NAME)
re: fclean

.PHONY: all clean fclean re