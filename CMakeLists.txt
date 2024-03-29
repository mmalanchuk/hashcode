cmake_minimum_required(VERSION 3.13)
project(hashcode C)

set(CMAKE_C_STANDARD 11)

include_directories(.)
include_directories(libftprintf/inc)
include_directories(libftprintf/inc/ft_printf)

add_executable(hashcode
        output.c
        output.h
        free_memory.c
        libftprintf/inc/ft_printf/colors.h
        libftprintf/inc/ft_printf/ft_printf.h
        libftprintf/inc/ft_printf/ft_printf_parsers.h
        libftprintf/inc/ft_printf/ft_printf_printers.h
        libftprintf/inc/ft_printf/ft_printf_structs.h
        libftprintf/inc/ft_printf/ft_printf_utils.h
        libftprintf/inc/btree.h
        libftprintf/inc/ctype.h
        libftprintf/inc/ft_math.h
        libftprintf/inc/get_next_line.h
        libftprintf/inc/libft.h
        libftprintf/inc/lists.h
        libftprintf/inc/mem.h
        libftprintf/inc/num.h
        libftprintf/inc/printers.h
        libftprintf/inc/queue.h
        libftprintf/inc/stack.h
        libftprintf/inc/str.h
        libftprintf/src/btree/btree_create_node.c
        libftprintf/src/btree/btree_del.c
        libftprintf/src/btree/btree_delone.c
        libftprintf/src/btree/btree_dfs_inorder.c
        libftprintf/src/btree/btree_dfs_postorder.c
        libftprintf/src/btree/btree_dfs_preorder.c
        libftprintf/src/btree/btree_insert_data.c
        libftprintf/src/btree/btree_level_count.c
        libftprintf/src/btree/btree_print.c
        libftprintf/src/btree/btree_search_data.c
        libftprintf/src/ctype/ft_is_empty.c
        libftprintf/src/ctype/ft_isalnum.c
        libftprintf/src/ctype/ft_isalpha.c
        libftprintf/src/ctype/ft_isascii.c
        libftprintf/src/ctype/ft_isdigit.c
        libftprintf/src/ctype/ft_isprint.c
        libftprintf/src/ctype/ft_tolower.c
        libftprintf/src/ctype/ft_toupper.c
        libftprintf/src/ft_printf/fpf_manage_char.c
        libftprintf/src/ft_printf/fpf_manage_number.c
        libftprintf/src/ft_printf/fpf_manage_string.c
        libftprintf/src/ft_printf/ft_printf.c
        libftprintf/src/ft_printf/ft_printf_core.c
        libftprintf/src/ft_printf/ft_printf_parsers.c
        libftprintf/src/ft_printf/ft_printf_printers.c
        libftprintf/src/ft_printf/ft_printf_utils.c
        libftprintf/src/get_next_line/get_next_line.c
        libftprintf/src/lists/ft_list_at.c
        libftprintf/src/lists/ft_list_last.c
        libftprintf/src/lists/ft_list_merge.c
        libftprintf/src/lists/ft_list_push_back.c
        libftprintf/src/lists/ft_list_push_front.c
        libftprintf/src/lists/ft_list_remove_if.c
        libftprintf/src/lists/ft_list_size.c
        libftprintf/src/lists/ft_list_sort.c
        libftprintf/src/lists/ft_lst_del_content.c
        libftprintf/src/lists/ft_lst_find.c
        libftprintf/src/lists/ft_lst_foreach.c
        libftprintf/src/lists/ft_lst_print.c
        libftprintf/src/lists/ft_lst_reverse.c
        libftprintf/src/lists/ft_lstadd.c
        libftprintf/src/lists/ft_lstdel.c
        libftprintf/src/lists/ft_lstdelone.c
        libftprintf/src/lists/ft_lstiter.c
        libftprintf/src/lists/ft_lstmap.c
        libftprintf/src/lists/ft_lstnew.c
        libftprintf/src/lists/ft_sorted_list_insert.c
        libftprintf/src/lists/ft_sorted_list_merge.c
        libftprintf/src/math/factorial.c
        libftprintf/src/math/ft_pow.c
        libftprintf/src/mem/ft_bzero.c
        libftprintf/src/mem/ft_memalloc.c
        libftprintf/src/mem/ft_memccpy.c
        libftprintf/src/mem/ft_memchr.c
        libftprintf/src/mem/ft_memcmp.c
        libftprintf/src/mem/ft_memcpy.c
        libftprintf/src/mem/ft_memdel.c
        libftprintf/src/mem/ft_memjoin.c
        libftprintf/src/mem/ft_memmove.c
        libftprintf/src/mem/ft_memset.c
        libftprintf/src/mem/ft_realloc.c
        libftprintf/src/num/ft_atoi.c
        libftprintf/src/num/ft_atoi_base.c
        libftprintf/src/num/ft_count_words.c
        libftprintf/src/num/ft_in_base.c
        libftprintf/src/num/ft_itoa.c
        libftprintf/src/num/ft_itoa_base.c
        libftprintf/src/num/ft_numlen.c
        libftprintf/src/num/ft_strtol.c
        libftprintf/src/printers/ft_perror.c
        libftprintf/src/printers/ft_putchar.c
        libftprintf/src/printers/ft_putchar_fd.c
        libftprintf/src/printers/ft_putendl.c
        libftprintf/src/printers/ft_putendl_fd.c
        libftprintf/src/printers/ft_putnbr.c
        libftprintf/src/printers/ft_putnbr_fd.c
        libftprintf/src/printers/ft_putstr.c
        libftprintf/src/printers/ft_putstr_fd.c
        libftprintf/src/queque/create_queue.c
        libftprintf/src/queque/del_queue.c
        libftprintf/src/queque/dequeue.c
        libftprintf/src/queque/enqueue.c
        libftprintf/src/queque/print_queue.c
        libftprintf/src/stack/stack_peek.c
        libftprintf/src/stack/stack_pop.c
        libftprintf/src/stack/stack_push.c
        libftprintf/src/stack/stack_size.c
        libftprintf/src/str/ft_str_count_occur.c
        libftprintf/src/str/ft_str_toupper.c
        libftprintf/src/str/ft_strcat.c
        libftprintf/src/str/ft_strchr.c
        libftprintf/src/str/ft_strclr.c
        libftprintf/src/str/ft_strcmp.c
        libftprintf/src/str/ft_strcpy.c
        libftprintf/src/str/ft_strdel.c
        libftprintf/src/str/ft_strdup.c
        libftprintf/src/str/ft_strequ.c
        libftprintf/src/str/ft_striter.c
        libftprintf/src/str/ft_striteri.c
        libftprintf/src/str/ft_strjoin.c
        libftprintf/src/str/ft_strjoin_free.c
        libftprintf/src/str/ft_strlcat.c
        libftprintf/src/str/ft_strlen.c
        libftprintf/src/str/ft_strmap.c
        libftprintf/src/str/ft_strmapi.c
        libftprintf/src/str/ft_strncat.c
        libftprintf/src/str/ft_strncmp.c
        libftprintf/src/str/ft_strncpy.c
        libftprintf/src/str/ft_strndup.c
        libftprintf/src/str/ft_strnequ.c
        libftprintf/src/str/ft_strnew.c
        libftprintf/src/str/ft_strnstr.c
        libftprintf/src/str/ft_strrchr.c
        libftprintf/src/str/ft_strrev.c
        libftprintf/src/str/ft_strsplit.c
        libftprintf/src/str/ft_strstr.c
        libftprintf/src/str/ft_strsub.c
        libftprintf/src/str/ft_strtrim.c
        main.c
        parsing.c
        parsing.h
        photo.h
        graph_builder.h
        graph_builder.c
        path_finder.h
        path_finder.c
        )
