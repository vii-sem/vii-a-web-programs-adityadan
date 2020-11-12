import threading
import time

def call(thread_name, delay):
    count = 0
    while count < 5:
        time.sleep(delay)
        count += 1
        print(thread_name, time.ctime(time.time()))

try:
    thread1 = threading.Thread(target=call, args=("Thread-1",2))
    thread2 = threading.Thread(target=call, args=("Thread-2",4))

    thread1.start()
    thread2.start()

except:
    print("Error: Unable to start threads")
