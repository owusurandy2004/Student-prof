name = input("What is your Name?")
age = int(input("What is your Age?"))

if age >= 18:
    age_status = "Adult"
else:
    age_status = "Minor"
    
gpa = float(input ("What is your GPA?"))

if gpa > 4.0:
    print ("Incorrct gpa")
elif gpa >= 3.5:
    deans_list = "Yes"
else:
    deans_list = "No"

courses = int(input("How many courses are you enrolled in?"))
string_list = []
for i in range(courses):
    s = input(f"Course # {i+1}:")
    string_list.append(s)
   
student_profile = {}
student_profile ["name"] = name
student_profile ["age"] = age
student_profile ["gpa"] = gpa
student_profile ["num_courses"] = courses
student_profile ["age_status"] = age_status
student_profile ["Deans_List"] = deans_list

print("========STUDENT PROFILE ======")
print(f"Name: {name}")
print(f"Age: {age}")
print(f"Age Status: {age_status}")
print(f"GPA: {gpa}")
print(f"Deans List: {deans_list}")
print(f"Courses:{int(courses)}")
print(f"Courses: {string_list}")
print("===============================")
