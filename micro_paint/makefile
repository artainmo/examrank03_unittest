all: run
re: fclean all

RM = rm -rf

run:
	@gcc -Wall -Wextra -Werror my/micro_paint.c -o my_micro_paint
	@gcc -Wall -Wextra -Werror micro_paint_tester/our_micro_paint.c -o our_micro_paint
	@python3 main.py

single:
	@gcc -Wall -Wextra -Werror my/micro_paint.c -o my_micro_paint
	@gcc -Wall -Wextra -Werror micro_paint_tester/our_micro_paint.c -o our_mini_paint
	@python3 single_test.py 2

set:
	pip3 install termcolor

clean:
	$(RM) __pycache__ utils/__pycache__

fclean:
	$(RM) my_micro_paint our_micro_paint
	$(RM) correct_log.txt errors_log.txt
	$(RM) __pycache__ micro_paint_tester/__pycache__ micro_paint_tester/examples/__pycache__
