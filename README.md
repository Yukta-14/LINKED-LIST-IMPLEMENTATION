# INTERNSHIP TASK - 02

# LINKED-LIST-IMPLEMENTATION

COMPANY: CODTECH IT SOLUTIONS

 NAME: YUKTA ANAND

 INTERN ID: CT04DN1416

 DOMAIN: C PROGRAMMING

 DURATION: 4 WEEKS

 MENTOR: NEELA SANTOSH


#  📘 Theory: Singly Linked List
A singly linked list is a dynamic data structure where:-

i) Each element (called a node) contains:-

   a) Data
   
   b)  A pointer to the next node

ii) The list is accessed via a pointer to the first node, called the head.

iii) Unlike arrays, linked lists don't require contiguous memory and can grow or shrink dynamically.

# 📂 Structure Definition

     c
     struct Node {
         int data;
         struct Node* next;
    };
This defines a Node structure with two members:-

 -> data: holds the integer value.

 -> next: points to the next node in the list.

# 🏗️ Node Creation

    c
    struct Node* createNode(int data);
Allocates memory for a new node, sets the data, and initializes next to NULL.

# ➕ Insertion Functions

1. At the Beginning

       c
       void insertAtBeginning(struct Node** head, int data);
-> A new node is created.

-> The new node's next is set to the current head.

-> The head pointer is updated to the new node.

2. At the End

       c
       void insertAtEnd(struct Node** head, int data);
-> A new node is created.

-> If the list is empty, it becomes the head.

-> Otherwise, traverse to the last node and attach the new node.

3. At a Given Position

       c
       void insertAtPosition(struct Node** head, int data, int position);
-> Handles inserting at the head (position == 0) directly.

-> Otherwise, traverses to the position before the target and adjusts the pointers.

-> If the position is invalid, prints "Position out of range".

# ❌ Deletion Functions

1. From the Beginning

       c
       void deleteFromBeginning(struct Node** head);
-> Removes the head node.

-> Moves the head pointer to the next node.

2. From the End

       c
       void deleteFromEnd(struct Node** head);
-> Traverses to the second-last node.

-> Frees the last node and sets next of the second-last to NULL.

3. From a Given Position

       c
       void deleteFromPosition(struct Node** head, int position);
-> Removes node at a specific position.

-> Handles edge cases (empty list or invalid position).

# 🔁 Traversal

     c
    void traverse(struct Node* head);
-> Iterates through each node.

-> Prints the data followed by an arrow.

# 🚀 Main Function Execution

    c
    int main()
Demonstrates the usage of all the functions in sequence:

(a) Inserts 10, 20, 30 at the end → 10 -> 20 -> 30

(b) Inserts 5 at beginning → 5 -> 10 -> 20 -> 30

(c) Inserts 25 at position 2 → 5 -> 10 -> 25 -> 20 -> 30

(d) Deletes from beginning → 10 -> 25 -> 20 -> 30

(e) Deletes from end → 10 -> 25 -> 20

(f) Deletes from position 1 → 10 -> 20

Each change is printed using traverse.

# ✅ Key Concepts Practiced

-> Dynamic memory allocation (malloc, free)

-> Pointers and pointer-to-pointer usage (struct Node**)

-> Linked list operations (insertion, deletion, traversal)

-> Edge case handling (empty list, invalid position)

 # OUTPUT 
 ![Image](https://github.com/user-attachments/assets/48618ee3-740d-4dc7-aec2-69852318a756)
