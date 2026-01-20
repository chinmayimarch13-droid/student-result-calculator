# Student Result Calculator

name = input("Enter student name: ")

marks = []
subjects = 5

for i in range(subjects):
    mark = int(input(f"Enter marks for subject {i+1}: "))
    marks.append(mark)

total = sum(marks)
percentage = total / subjects

if percentage >= 90:
    grade = "A"
elif percentage >= 75:
    grade = "B"
elif percentage >= 60:
    grade = "C"
elif percentage >= 40:
    grade = "D"
else:
    grade = "Fail"

print("\n----- RESULT -----")
print("Name:", name)
print("Total Marks:", total)
print("Percentage:", percentage)
print("Grade:", grade)# student-result-calculator
