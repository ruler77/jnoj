all: src/dispatcher.c src/judge.c
	gcc -std=gnu99 -Wall -c -I/usr/local/mysql/include/mysql -I/usr/include/mysql  src/dispatcher.c
	gcc -std=gnu99 -Wall -o dispatcher dispatcher.o -L/usr/local/mysql/lib/mysql -L/usr/lib/mysql  -L/usr/lib64/mysql  -lmysqlclient

	gcc -std=gnu99 -Wall -c -I/usr/local/mysql/include/mysql -I/usr/include/mysql src/judge.c src/cJSON.c
	gcc -std=gnu99 -Wall -o judge judge.o cJSON.o -L/usr/local/mysql/lib/mysql -L/usr/lib/mysql  -L/usr/lib64/mysql -lmysqlclient
	rm judge.o dispatcher.o cJSON.o