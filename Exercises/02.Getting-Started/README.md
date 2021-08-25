## Chapter 2. Getting Started
# 2.1: Insertion Sort
### 2.1.1:
Iteration 1: [31, 41, 59, 26, 41, 58]
Iteration 2: [31, 41, 59, 26, 41, 58]
Iteration 3: [26, 31, 41, 59, 41, 58]
Iteration 4: [26, 31, 41, 41, 59, 58]
Iteration 5: [26, 31, 41, 41, 58, 59]
#### Python Code
    def  insertionSort(A):
	    for  i  in  range(1, len(A)):
		    key = A[i]
		    j = i - 1
		    while  j > -1  and  A[j] > key:
			    A[j+1] = A[j]
			    j = j - 1
		    A[j + 1] = key    
	    return  A

### 2.1.2:
    def  insertionSortDescendingOrder(A):
    	for  i  in  range(1, len(A)):
    		key = A[i]
    		j = i - 1
    		while  j > -1  and  A[j] < key:
    			A[j+1] = A[j]
    			j = j - 1
    		A[j + 1] = key
	    return  A

### 2.1.3:
#### Python Code
    def  linearSearch(A, v):
    	for  i  in  range(len(A)):
    		if  v == A[i]:
    			return  i
    	return  None
    
**Loop invariant:** At the start of each iteration of the **for** loop, the subarray `A[1 ... i - 1]` consists of elements that are different than v.
**Initialization:** Before the first loop iteration (i = 1), the subarray is the empty array.
**Maintenance:**  During each loop iteration, we compare  v  with  A[i]. If they are the same, we return  i, which is the correct result. Otherwise, we continue to the next iteration of the loop. At the end of each loop iteration, we know the subarray  A[1..i] does not contain  v, so the loop invariant holds true. Incrementing  i for the next iteration of the  **for**  loop then preserves the loop invariant.
**Termination:**  The loop terminates when  i > A.length = n. Since  i increases by  1, we must have  i = n + 1 at that time. Substituting  n + 1, for  i in the wording of the loop invariant, we have that the subarray  A[1..n] consists of elements that are different than  v. Thus, we return  NIL. Observing that  A[1..n], we conclude that the entire array does not have any element equal to  v. Hence the algorithm is correct.
### 2.1.4:
**Input:** An array of boolean digits A = [a1, a2, ..., an] and an array of boolean digits B = [b1, b2, ..., bn] each representing an integer stored in binary format and each of length n.
**Output:** An array C = [c1, c2, ..., cn] represents the boolean digits of the summation of the two boolean input arrays.

#### Python Code

    def  addBinary(A, B):
	    C = [0] * (len(A) + 1)
	    carry = 0
	    for  i  in  range(len(A) - 1, -1, -1):
		    C[i+1] = (A[i] + B[i] + carry) % 2
		    carry = (A[i] + B[i] + carry) // 2
	    C[i] = carry
	    return  C

