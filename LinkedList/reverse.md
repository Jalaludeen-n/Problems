it is the sample input 1 -> 2 -> 3 -> 4 -> 5
reuslt must be like this 5 -> 4 -> 3 -> 2 -> 1

1) take first node and set first node next is null
     temp = head;
     temp.next = null;
   cons :
        if we change next as null we can't access next node of the head beacause of it by reference.
    solution
        take a copy of next then update the result with result node
        we point head
        temp = head;
        we point head.next
        next = head.next;
        and change temp  next as null
        temp.next = null;
        as result we got two linked list one with the first value next with all other values
    
    result  = head;

    result 1 -> null
    result next = null
    head 1 2 3 4 5
    1 2 3 4 5
    1 2 3 4 5
     result 1 -> null
     next 2 3 4 5
     prv 2 3 4 5
     prv 2 -> 1 -> null 




