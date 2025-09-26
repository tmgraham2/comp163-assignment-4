# comp163-assignment-4
student_name = "Tashe Graham"
current_gpa = 3.85
study_hours = 20
social_points = 30
stress_level = "Medium"
print("Hello", student_name, "these are you're starting stats!")
print("\nCurrent GPA:", current_gpa)
print("\nStudy Hours:", study_hours)
print("\nSocial Points:", social_points)
print("\nStress Level:", stress_level)

print("Choose your course load: ")
print("A) Light (12 credits)")
print("B) Standard (15 credits)")
print("C) Heavy (18 credits)")

choice = input("Your choices: ")

if choice == "A":
    print("You've chosen a Light course load.")
    if current_gpa >= 3.0:
        study_hours = 10
        stress_level = "Low"
    else: 
        study_hours = 15
        stress_level = "Medium"
    print(f"Your study hours: {study_hours} \nYour stress level: {stress_level}")

elif choice == "B":
    print("You've chosen a standard course load.")
    if current_gpa >= 3.5:
        study_hours = 15
        stress_level = "Medium"
    else:
        study_hours = 20
        stress_level = "High"
    print(f"Your study hours: {study_hours} \nYour stress level: {stress_level}")

elif choice == "C":
    print("You've chosen a heavy course load.")
    if current_gpa >= 3.8:
        study_hours = 20
        stress_level = "High"
    else:
        study_hours = 25
        stress_level = "High"
    print(f"Your study hours: {study_hours} \nYour stress level: {stress_level}")

else:
    print("Your information is unavailable.")

