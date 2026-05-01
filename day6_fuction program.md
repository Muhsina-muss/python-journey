def get_grade_marks(marks,name):
    if marks>100 or marks<0:
       result= "hello " +name+ "invalid"
       return result
    elif marks >= 75:
       return "gradeA"
    elif marks >=60:
       return "gradeB"
    elif marks >=50:
       return "gradeC"
    
    else:
        result="hello " +name+ "you are failed "
        return result
grade=get_grade_marks(150,"muhsina")
print(grade)
    
