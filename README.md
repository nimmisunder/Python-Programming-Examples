# Python-Programming-Examples

1.Given the participants' score sheet for your University Sports Day, 
you are required to find the runner-up score. You are given  scores. Store them in a list and find the score of the runner-up.

     n = int(input())
     arr = list(map(int, input().split()))    
     sorted_a = sorted(arr)   
     unique_scores = []
    
     for num in sorted_a:
        if num not in unique_scores:
            unique_scores.append(num)
     print(unique_scores[-2])
                             OR
     n = int(input())
     arr = map(int, input().split()) 
     sorted_a = sorted(set(arr))
     print(sorted_a[-2])

2.You are given a string and your task is to swap cases. In other words, convert all lowercase letters to uppercase letters and vice versa.

For Example:

Www.HackerRank.com → wWW.hACKERrANK.COM
Pythonist 2 → pYTHONIST 2  


                def swap_case(s):
              ns=''
              for ch in s:
                  if ch.isupper():
                      ns+=ch.lower()
                  elif ch.islower():
                      ns+=ch.upper()
                  else:
                      ns+=ch
                  
                      
              return ns
          
               if __name__ == '__main__':
                   s = input()
                   result = swap_case(s)
                   print(result)

How do you reverse an array in Python?
          Method 1: Using slicing
          arr = [1, 2, 3, 4, 5]print(arr[::-1])



          Output:
          [5, 4, 3, 2, 1]


          Method 2: Using reverse()
          arr = [1, 2, 3, 4, 5]arr.reverse()print(arr)



          Method 3: Using reversed()
          arr = [1, 2, 3, 4, 5]result = list(reversed(arr))print(result)



          Interview distinction:
          - reverse() modifies the original list.
          - reversed() returns an iterator.
          - [::-1] creates a reversed copy.

     How do you update a dictionary?
           employee = {
                   "name": "John",
                   "salary": 30000
               }
               
               employee["salary"] = 40000
               
               employee["department"] = "IT"
               
               print(employee)


Two Sum Problem
Important coding question
Question: Given an array of integers and a target value, find the indices of two numbers whose sum equals the target.
               
               Example:
               nums = [2, 7, 11, 15]target = 9
               
               
               
               Expected output:
               [0, 1]
               
               
               Because:
               nums[0] + nums[1]
               2 + 7 = 9
               
               
               Solution using a dictionary (Hash Map):
               def two_sum(nums, target):    seen = {}    for i, num in enumerate(nums):        difference = target - num        if difference in seen:            return [seen[difference], i]        seen[num] = i    return []nums = [2, 7, 11, 15]print(two_sum(nums, 9))
               
               
               
               Output:
[0, 1]
