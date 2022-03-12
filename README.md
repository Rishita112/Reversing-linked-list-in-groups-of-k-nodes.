# Reversing-linked-list-in-groups-of-k-nodes.
The head of a linked list is given and we have to reverse the nodes of the list k at a time, and return the modified list.Here,k is a positive integer and is less than or equal to the length of the linked list. 
If the number of nodes is not a multiple of k then left-out nodes in the end should remain as it is i.e will not be reversed.

First we declare a struct Listnode which have int val and next pointer.
A count function is given which calculates the length of the list.

After that there is  reverseKGroup and reverse functions.In reverseKGroup function we first check whether head is null or not.If it is not null we will calculate the length of the list and divide it by k to find number of group
that has to reversed.We then reverse group of k nodes in the reverse function.The reverse funcrion returns the vector of size two,where first element of vector i.e v[0] points to head of that group whereas second element i.e v[1]
points to next node of the upcoming group.Also the prev pointer points to the last node of the previous group of k nodes and the nxt pointer points to the first node of the upcoming group.In this way we reverse every group 
containing k nodes and leave the remaining unchanged.
