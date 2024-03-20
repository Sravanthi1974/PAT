class Node:
    def __init__(self,data):
        self.data= data
        self.next = None
class SpecialStack:
    def __init__(self):
        self.top=None
        self.minEle=None
    def push(self,data):
        newNode=Node(data)
        if self.top == None:
            self.top=newNode
            self.minEle=data
        else:
            if data < self.minEle:
                newNode.data= 2*data-self.minEle
                self.minEle=data
            newNode.next=self.top
            self.top=newNode
    print(f"pushed: {data}, peak: {self.top.data}, min: {self.minEle}")
    def pop(self):
        if self.top is None :
            raise IndexError("pop from empty stack")
        temp= tem.top.data
        self.top= self.top.next
        if temp<self.minEle:
            minRemoved= self.minEle
            self.minEle= 2*self.minEle - temp
            print(f"popped: {data}, peak: {self.top.data if self.top else None}, min: {self.minEle}")
            return minRemoved
        else:
            print(f"popped: {data}, peak: {self.top.data if self.top else None}, min: {self.minEle}")
    def isEmpty(self):
        return self.top is None
    def getMin(self):
        if self.top is None:
            raise IndexError ("get min from empty stack")
        return self.minEle
        
        
#create a special stack object
special_stack= SpecialStack()

#insert the data into the special stck using push
data=[3,5,2,1,1,-1]
for item in data:
    special_stack.push(item)

#pop elements from special stack
while not special_stack.isEmpty():
    special_stack.pop()