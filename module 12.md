EXP NO 26: 

C PROGRAM TO DISPLAY STACK ELEMENTS USING LINKED LIST.  

Aim: 

To write a C program to display stack elements using linked list. 

Algorithm: 

1. Define a structure Node with two members: data to store the integer value and 
next to point to the next node in the linked list. 
2. Declare a global variable head representing the starting node of the linked list. 
3. Define a function display to print the elements of the linked list. 
4. Declare a pointer p and initialize it with the head of the linked list. 
5. Use a while loop to traverse the linked list: 
6. Print the data of the current node. 
7. Move to the next node using the next pointer. 

Program: 
```
struct Node    
{   
char data[100];   
struct Node *next;   
}*head;   
void display()   
{   
} 
struct Node * ptr=head; 
while(ptr!=NULL) 
{ 
} 
printf("%s\n",ptr->data); 
ptr=ptr->next;
```


Output: 

![Screenshot 2025-05-11 100358](https://github.com/user-attachments/assets/3004096c-70b0-4c67-8c35-5fa0ba07c960)


Result:  

Thus, the program to display stack elements using linked list is verified successfully. 

EXP.NO 27:  

C PROGRAM TO POP AN ELEMENT FROM THE GIVEN STACK USING LINKED LIST.  

Aim:

To write a C program to pop an element from the given stack using liked list. 

Algorithm: 

1. Check for Empty Stack 
2. If head is equal to NULL, Print "Stack is empty." 
3. Else Proceed to the next step. 
4. Set head to point to the next node in the stack. 

Program: 
```
struct Node    
{   
char data[100];   
struct Node *next;   
}*head;   
void pop()   
{  
if(head==NULL) 
    { 
        printf("stack is empty"); 
    } 
    else 
    { 
        struct Node * ptr=head; 
        head=head->next; 
        free(ptr); 
        ptr=NULL; 
    } 
}
```

Output: 

![Screenshot 2025-05-11 100408](https://github.com/user-attachments/assets/aec4395e-a7de-4fd4-b424-0699aeb76916)

 
Result: 

 Thus, the program to pop an element from the given stack using liked list is verified 
successfully. 
 
 
 
EXP NO:28  

C PROGRAM TO DISPLAY QUEUE ELEMENTS USING LINKED LIST.  

Aim:

To write a C program to display queue elements using linked list. 
 
 
Algorithm: 

1. Check if Queue is Empty 
2. Display Queue Elements 
3. Print the data of the current node pointed to by front 
4. Update front to point to the next node. 
5. End the display function. 


Program: 
```
struct Node 
{ 
   char data; 
   struct Node *next; 
}*front=NULL,*rear=NULL; 
void display() 
{ 
    if(front==NULL) 
    { 
        printf("queue is empty"); 
        return; 
    } 
    printf("queue elements:\n"); 
    struct Node *ptr=front; 
    while(ptr!=NULL) 
    { 
        printf("%c\n",ptr->data); 
        ptr=ptr->next; 
} 
}
```


Output: 

![Screenshot 2025-05-11 100416](https://github.com/user-attachments/assets/d1ca3d56-8058-45ae-8e5a-2910096df11a)


Result:  

Thus, the program to display queue elements using linked list is verified successfully. 



EXP NO:29 

C PROGRAM TO INSERT ELEMENTS IN QUEUE USING LINKED LIST 


Aim:

To write a C program to insert elements in queue using linked list 


Algorithm: 

1. Allocate Memory for New Node 
2. Set Data and Next Pointer 
3. Check if Queue is Empty 
4. Set both front and rear to point to the new node p. 
5. Set the next pointer of the current rear to point to the new node p. 
6. End of Enqueue Operation 

Program: 
```
struct Node 
{ 
   int data; 
   struct Node *next; 
}*front=NULL,*rear=NULL; 
void enqueue(int data) 
{ 
    struct Node *ptr=malloc(sizeof(struct Node)); 
    ptr->data=data; 
    ptr->next=NULL; 
    if(front==NULL) 
    { 
        front=rear=ptr; 
    } 
    else 
    { 
        rear->next=ptr; 
        rear=ptr; 
    } 
}
```
Output:

![Screenshot 2025-05-11 100423](https://github.com/user-attachments/assets/8973c16b-8c84-4895-9f9b-d5070464037c)

 
Result:

Thus, the program to insert elements in queue using linked list is verified successfully. 


EXP NO:30  

C FUNCTION TO FIND THE PEEK OF QUEUE USING LINKED LIST. 

Aim: 

The aim of this function is to retrieve the "peek" (the front element) of a queue 
implemented using a linked list 

Algorithm: 

1. Check if the queue is empty: o If the queue is empty (i.e., the front pointer is 
NULL), return an error or a message indicating that the queue is empty. 
2. Access the front element: o If the queue is not empty, return the data stored in 
the front node of the linked list (i.e., the element at the head of the queue). 


Program: 
```
struct Node 
{ 
float data; 
struct Node *next; 
}*front=NULL,*rear=NULL; 
void peek() 
{ 
} 
struct Node *ptr=front; 
printf("%.2f",ptr->data); 
ptr=ptr->next;

``` 
Output: 

![Screenshot 2025-05-11 100431](https://github.com/user-attachments/assets/ac5a1554-15c5-408e-b3fa-5a7785cdc7e0)

 
Result: 

Thus, the program to retrieve the "peek" (the front element) of a queue implemented 
using a linked list is verified successfully. 
 
