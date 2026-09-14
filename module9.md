EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

Aim:
To write a C program to display stack elements using an array.
Algorithm:
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
Program:
```

#include <stdio.h>

int stack[5] = {10, 20, 30, 40, 50};
int top = 4;

void display() {
    int i;

    printf("Stack elements are:\n");

    for (i = top; i >= 0; i--) {
        printf("%d\n", stack[i]);
    }
}

int main() {
    display();

    return 0;
}



```
Output:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3db18713-e46d-40a7-a5a9-bfd6f3e4c3f6" />



Result:
Thus, the program to display stack elements using an array is verified successfully.
 

EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.
Aim:
To create a C program to push the given element in to a stack using array.
Algorithm:
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
Program:
```


#include <stdio.h>

int stack[5];
int top = -1;

void push(int value) {
    if (top == 4) {
        printf("Stack is full.\n");
    } else {
        top++;
        stack[top] = value;
        printf("%d pushed into stack\n", value);
    }
}

int main() {
    push(10);
    push(20);
    push(30);

    return 0;
}


```


Output:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/01979774-bc63-40cb-ac44-d88c1b5bf8e4" />




Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
Aim:
To write a C program to display queue elements using array

Algorithm:
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
Program:
 ```


#include <stdio.h>

int queue[5] = {10, 20, 30, 40, 50};
int front = 0;
int rear = 4;

void display() {
    int i;

    printf("Queue elements are:\n");

    for (i = front; i <= rear; i++) {
        printf("%d\n", queue[i]);
    }
}

int main() {
    display();

    return 0;
}



```


Output:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/5dd9a46c-6d77-48e6-8b1f-d4d60ca84c8d" />



Result:
Thus, the program to display queue elements using array is verified successfully.


 
EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
Aim:
To write a C program to insert elements in queue using array.

Algorithm:
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

Program:
```



#include <stdio.h>

int queue[5];
int front = -1;
int rear = -1;

void enqueue(int value) {
    if (rear == 4) {
        printf("Queue is full.\n");
    } else {
        if (front == -1)
            front = 0;

        rear++;
        queue[rear] = value;

        printf("%d inserted into queue\n", value);
    }
}

int main() {
    enqueue(10);
    enqueue(20);
    enqueue(30);

    return 0;
}



```
Output:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ce957702-eb86-4f1b-a4ff-63b5d3998708" />



Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY



Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



Program:

```

#include <stdio.h>

int queue[5] = {10, 20, 30, 40, 50};
int front = 0;
int rear = 4;

void deleteElement() {
    if (front == -1) {
        printf("Queue is empty.\n");
    } else {
        printf("Deleted element: %d\n", queue[front]);

        front++;

        if (front > rear) {
            front = -1;
            rear = -1;
        }
    }
}

void display() {
    int i;

    if (front == -1) {
        printf("Queue is empty.\n");
    } else {
        printf("Queue elements are:\n");

        for (i = front; i <= rear; i++) {
            printf("%d\n", queue[i]);
        }
    }
}

int main() {
    printf("Before deletion:\n");
    display();

    deleteElement();

    printf("\nAfter deletion:\n");
    display();

    return 0;
}




```

Output:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c684950d-4482-4f4f-9315-e276ee8af9d2" />

Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
