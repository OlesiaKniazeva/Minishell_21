NAME = libft.a

S_DIR = srcs/

SRCS =	ft_memset.c			ft_bzero.c\
		ft_memccpy.c		ft_strmapi.c\
		ft_memcmp.c			ft_strlen.c\
		ft_strchr.c			ft_strrchr.c\
		ft_strnstr.c		ft_strncmp.c\
		ft_isalpha.c		ft_isdigit.c\
		ft_isascii.c		ft_isprint.c\
		ft_tolower.c		ft_calloc.c\
		ft_substr.c			ft_strjoin.c\
		ft_strlcat.c		ft_itoa.c\
		ft_putchar_fd.c		ft_putstr_fd.c\
		ft_putnbr_fd.c		ft_strtrim.c\
		ft_memmove.c		ft_memcpy.c\
		ft_split.c			ft_memchr.c\
		ft_strlcpy.c		ft_atoi.c\
		ft_isalnum.c		ft_toupper.c\
		ft_strdup.c			ft_putendl_fd.c\
		ft_lstnew.c			ft_lstsize.c\
		ft_lstlast.c		ft_lstadd_front.c\
		ft_lstdelone.c		ft_lstadd_back.c\
		ft_lstclear.c		ft_lstiter.c\
		strchr_len.c

OBJS = $(SRCS:.c=.o)

OBJS_LIST = $(addprefix $(S_DIR), $(OBJS))

CC = gcc

RM = rm -f

INCL = ../includes

HEADER = libft.h

H_PATH = $(INCL)/$(HEADER)

CFLAGS =  -g -Wall -Wextra -Werror -I $(INCL)

%.o: %.c $(H_PATH)
	$(CC) $(CFLAGS) -c $< -o $@

.PHONY: all clean fclean re bonus

all: $(NAME)

$(NAME): $(OBJS_LIST)
			ar rc $(NAME) $(OBJS_LIST)

clean:
		$(RM) $(OBJS)

fclean:	clean
		$(RM) $(NAME)

re:	fclean all

