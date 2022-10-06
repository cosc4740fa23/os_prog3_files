CC=g++
#CFLAGS = -pthread -std=c++11
CFLAGS = -pthread 

all: simple oddeven_c oddeven_p oddeven buffer buffer_param buffer_sm dock atomic

simple: thread_simple.cpp
	$(CC) $(CFLAGS)  -o simple thread_simple.cpp

oddeven_c: thread_oddeven_cout.cpp
	$(CC) $(CFLAGS)  -o oddeven_c  thread_oddeven_cout.cpp

oddeven_p: thread_oddeven_printf.cpp
	$(CC) $(CFLAGS)  -o oddeven_p  thread_oddeven_printf.cpp

oddeven: semaphore_mutex_oddeven.cpp
	$(CC) $(CFLAGS)  -o oddeven semaphore_mutex_oddeven.cpp

buffer:  semaphore_buffer.cpp
	$(CC)  $(CFLAGS) -o buffer semaphore_buffer.cpp

buffer_param: semaphore_buffer_param.cpp
	$(CC) $(CFLAGS) -o buffer_param semaphore_buffer_param.cpp

buffer_sm:  semaphore_mutex_buffer.cpp
	$(CC) $(CFLAGS) -o buffer_sm  semaphore_mutex_buffer.cpp

dock: semaphore_mutex_dock.cpp
	$(CC) $(CFLAGS) -o dock semaphore_mutex_dock.cpp

atomic:  atomic_example.cpp
	$(CC) $(CFLAGS) -o atomic  atomic_example.cpp

clean: 
	rm -f simple oddeven_c oddeven_p oddeven buffer buffer_param buffer_sm dock atomic
