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
study_options = ["Programming", "Math", "English", "History"]

choice2 = input("Enter your choice of study from the list: Programming, Math, English, or History")

#Recommended studying techniques for each study option
if choice2 in study_options:
    print(f"You have chosen {choice2}.")
    if (choice2 in ["Programming"]) and (current_gpa >= 3.5 and social_points >= 25):
        print("Using interactive learning platforms like Zybooks and taking university courses are recommended.")
    elif (choice2 in ["Math"]) and (current_gpa >= 3.5 and social_points >= 25):
        print("Solving problems and using online tools like KhanAcademy and Youtube is recommended.")
    elif (choice2 in ["English"]) and (current_gpa >= 3.5 or social_points >= 25):
        print("Using flashcards and constanly reviewing notes are recommended.")
    elif (choice2 in ["History"]) and (current_gpa >= 3.5 or social_points >=25):
        print("Making accurate timelines and graphic organizers are recommended.")
    elif choice2 not in study_options:
        print("Invalid study options.")
else:
    print("Please choose a valid study option from the list: Programming, Math, English, or History.")



    
