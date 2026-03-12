# Data-structure-practical-program18-
class Queue:
    def __init__(self):
        self.queue = []

    def enqueue(self, item):
        self.queue.append(item)
        print(item, "added to queue")

    def dequeue(self):
        if len(self.queue) == 0:
            print("Queue is empty")
        else:
            print("Removed:", self.queue.pop(0))

    def display(self):
        print("Queue elements:", self.queue)


q = Queue()

q.enqueue(10)
q.enqueue(20)
q.enqueue(30)

q.display()

q.dequeue()
q.display()
10 added to queue
20 added to queue
30 added to queue
Queue elements: [10, 20, 30]
Removed: 10
Queue elements: [20, 30]
