For each of the methods associated with each data structure, classify it based on its worst-case runtime, using Big O notation.

## Linked List

1) What is the runtime complexity of `add_to_tail`?
- O(c), we can reference our tail property and quickly add it.
  
1a) What if our list implementation didn't have a reference to the tail of the list in its constructor? What would be the runtime of the `add_to_tail` method?
- O(n), we have to go through the whole list to get to the end to add to the tail.

2) What is the runtime complexity of `remove_head`?
- O(c), we have a reference to the head and can quickly remove it.

3) What is the runtime complexity of `contains`?
- O(n), we have to check all the items in the list to see if it contains the number.

4) What is the runtime complexity of `get_max`?
- O(n), we have to go through every value to compare to the number in storage.

## Queue

1) What is the runtime complexity of `enqueue`?
- O(c), since we already have the tail reference.

2) What is the runtime complexity of `dequeue`?
- O(c), since we already have the head reference.

3) What is the runtime complexity of `len`?
- O(c), since we are using a self.size to keep track.

## Binary Search Tree

1) What is the runtime complexity of `insert`? 
- O(logn), it has to traverse half trees to find its place.

2) What is the runtime complexity of `contains`?
- O(logn), it has to traverse half trees to find the target value.

3) What is the runtime complexity of `get_max`? 
- O(logn), it has to traverse half trees all the way through to make sure it's the highest value.

## Heap

1) What is the runtime complexity of `_bubble_up`?
- O(logn), goes through half tree upwards pattern in order to swap the higher parent value with current value.

2) What is the runtime complexity of `_sift_down`?
- O(logn), goes through half tree downwards pattern in order to swap highest child value with current value.

3) What is the runtime complexity of `insert`?
- O(logn), regular insert is a simple append so O(c) but goes through half tree pattern when doing _bubble_up in order to heapify.

4) What is the runtime complexity of `delete`?
- O(logn), delete is just a simple swap so O(c) but goes through half tree pattern when doing _sift_down in order to correct the tree.

5) What is the runtime complexity of `get_max`?
- O(c), always the same operation.

## [Stretch Goal] Doubly Linked List

1. What is the runtime complexity of `ListNode.insert_after`?

2. What is the runtime complexity of `ListNode.insert_before`?

3. What is the runtime complexity of `ListNode.delete`?

4. What is the runtime complexity of `DoublyLinkedList.add_to_head`?

5. What is the runtime complexity of `DoublyLinkedList.remove_from_head`?

6. What is the runtime complexity of `DoublyLinkedList.add_to_tail`?

7. What is the runtime complexity of `DoublyLinkedList.remove_from_tail`?

8. What is the runtime complexity of `DoublyLinkedList.move_to_front`?

9. What is the runtime complexity of `DoublyLinkedList.move_to_end`?

10. What is the runtime complexity of `DoublyLinkedList.delete`?

    a. Compare the runtime of the doubly linked list's `delete` method with the worst-case runtime of the JS `Array.splice` method. Which method generally performs better?