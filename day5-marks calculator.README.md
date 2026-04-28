name = input("Enter your name: ")
marks = []

print("Enter marks for 5 subjects:")
for i in range(5):
    mark = int(input("Subject " + str(i+1) + ": "))
    marks.append(mark)

# BOX 2: PROCESS - This is the new part
total = 0 # Step 1: Make empty total box
highest = marks[0] # Step 2: Assume first mark is highest for now
lowest = marks[0] # Step 3: Assume first mark is lowest for now

for mark in marks: # Step 4: Check each mark one by one
    total = total + mark # Add this mark to total

    if mark > highest: # If this mark is bigger than our highest
        highest = mark # Then this mark becomes the new highest

    if mark < lowest: # If this mark is smaller than our lowest
        lowest = mark # Then this mark becomes the new lowest

percentage = total / 5 # Step 5: Average of 5 subjects

# BOX 3: OUTPUT - Show results
print("\n--- REPORT CARD ---")
print("Name:", name)
print("Marks:", marks)
print("Total:", total, "/ 500")
print("Percentage:", percentage, "%")
print("Highest mark:", highest)
print("Lowest mark:", lowest)

if percentage >= 90:
    print("Grade: A+")
elif percentage >= 75:
    print("Grade: A")
elif percentage >= 60:
    print("Grade: B")
elif percentage >= 50:
    print("Grade: C")
elif percentage >= 40:
    print("Grade: D")
else:
    print("Grade: E - Failed")
