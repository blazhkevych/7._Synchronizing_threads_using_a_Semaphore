# 7. Синхронизация потоков с помощью семафора

Разработать WinForms-приложение, которое будет использовать 
объект-семафор следующим образом. По нажатию на кнопку "Создать поток" 
создается новый поток и помещается в первый список, где находятся все 
созданные потоки. Порядковый номер потока берется от 1 и увеличивается на 
один. При двойном клике на потоке, поток перемещается в список 
ожидающих потоков, где он будет находиться до тех пор, пока в семафоре не 
освободится для него место. Как только такое место освободилось, поток 
перемещается из списка ожидания в список рабочих потоков и приступает к 
работе. Работа заключается в том, чтобы увеличивать локальный счетчик 
каждого потока на единицу в секунду и отображать это значение. При 
двойном клике по потоку в списке рабочих потоков, поток прекращает свою 
работу, удаляется из списка и освобождает место для очередного 
ожидающего потока. Количество свободных мест задается в счетчике. При 
изменении счетчика более "старые" потоки покидают список, если произошло 
уменьшение счетчика, или же добавляются новые "ожидающие" потоки при 
увеличении значения счетчика.

# 7. Synchronize threads using a semaphore

Develop a WinForms application that will use
semaphore object as follows. By clicking on the button "Create stream"
a new thread is created and placed in the first list where all
created streams. The stream sequence number is taken from 1 and incremented by
one. When double clicking on a stream, the stream is moved to the list
waiting threads, where it will be until the semaphore is not
make room for him. As soon as such a place was vacated, the flow
moves from the waiting list to the list of worker threads and proceeds to
work. The job is to increment the local counter
per thread per unit per second and display that value. At
double click on a thread in the list of worker threads, the thread stops its
work is removed from the list and frees up space for the next
waiting thread. The number of free places is set in the counter. At
change of the counter "older" threads leave the list if
decrement the counter, or new "waiting" threads are added when
increasing the value of the counter.

![image](https://user-images.githubusercontent.com/65856963/228859867-0c347e19-d75b-4524-8def-2b207d51daac.png)
