#this is comment sym...
count_words: count_words.o lexer.o -lfl
	gcc $^ -o $@
count_words.o: count_words.c
	gcc -c $<
lexer.o: lexer.c
	gcc -c $<
lexer.c: lexer.l
	flex -t $< > $@
clean:
	rm *.o lexer.c count_words
.PHONY:clean
