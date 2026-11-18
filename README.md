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
