headPtr is in main on stack not pointing to anything. Its a NULL pointer. Calling addNode in this state would pass NULL into the function. 

>#include <stdio.h>
>#include <stdlib.h>
>
>//Struct Definition
>struct NodeType{
>	char costume[30];
	  double cost;
	  struct NodeType* nextPtr; // Pointer to next node
};
>
// Rename the struct
typedef struct NodeType Node;
>
// function prototype
void addNode(Node* headPtr){
>
}
>
int main(){
  // declare variables
  Node* headPtr = NULL;   // Initialize to empty list
>
  return 0;
}

Instead of passing NULL we want to pass the address of headPtr. To do this, we need to pass another pointer.

>	// function prototype
	void addNode(Node** headPtr){
	}

