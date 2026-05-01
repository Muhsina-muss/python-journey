def check_pass(marks):
    if marks >= 40:
       return True
    elif marks < 40:
       return False
    
result1 = check_pass(75)  
print("result1 is " ,result1)
result2 = check_pass(35)
print("result2 is ",result2)
