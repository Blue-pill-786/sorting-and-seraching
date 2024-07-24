def __init__(self, data):
        self.data = data
        self.next = None



def sortedinsert(head_ref , new_node_data):
   
    current = None
    new_node = Node(new_node_data)
   
    if head_ref == None or head_ref.data>= new_node.data:
        new_node.next = head_ref
        head_ref = new_node
    else:
        current = head_ref
        while current.next != None and current.next.data< new_node.data:
            current = current.next
       
        new_node.next = current.next
        current.next = new_node    
    return head_ref
   
   

def printlist(a):
    temp = a
    while temp != None:
        print(temp.data, end=" ")
        temp = temp.next

def push(head_ref, new_data):
    new_node = Node(new_data)
   
    new_node.next = head_ref
    head_ref = new_node
    return head_ref


   
def search(head, node_data):
    c=head
    while c.next != None:
        if c.data!=node_data:
            c=c.next
        elif c.data == node_data:
            return True
    return False

   


nodewithoutsort = None
nodewithsortedinsert = None
a = int(input("enter the number of nodes: "))
b=0
while b<a:
    c= int(input("enter the new node: "))
    nodewithoutsort = push(nodewithoutsort, c)
    nodewithsortedinsert = sortedinsert(nodewithsortedinsert, c)
   
    b+=1
print("without sorted insert" )
printlist(nodewithoutsort)
print()
print("with sorted insert")
printlist(nodewithsortedinsert)

print()
sea = int(input("enter the data to search"))
s = search(nodewithsortedinsert, sea)
print(s)
