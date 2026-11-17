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
