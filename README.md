# comp163-personal-portfolio
# PERSONAL ACADEMIC & LIFE PORTFOLIO
# =========================

# --- Basic Info ---
full_name = "Che Mullins"
student_email = "cdmullins@ncat.edu"
hometown = "Washington, D.C"
graduation = "Spring 2029"
major = "Computer Science"

# --- Coursework & Academics ---
course_list = ["COMP 163", "COMP 121", "MATH 131", "ENG 100", "GEEN 111"]
completed_courses = ["IB Biology", "IB Math", "IB Art", "IB Spanish 6", "IB World History"]

credit_hours = [3, 3, 3, 3, 3]   # all courses assumed 3 credits
gpa_history = [2.9, 3.9, 4.2, 4.6]

credit_dict = {"COMP 163": 3, "COMP 121": 3, "MATH 131": 3, "ENG 100": 3, "GEEN 111": 3}
professors_dict = {"COMP 163": "Prof. Rhodes", "COMP 121": "Prof. Allen",
                   "MATH 131": "Prof. Gibson", "ENG 100": "Prof. Rush", "GEEN 111": "Prof. Parrish"}
rooms_dict = {"COMP 163": "M-Eric 3", "COMP 121": "Marteena 105",
              "MATH 131": "Marteena 224", "ENG 100": "Crosby 121", "GEEN 111": "McNair 210"}

# --- Budget & Study ---
budget_dict = {"Food": 350, "Entertainment": 200, "Books": 125, "Transportation": 100}
study_dict = {"Programming": 10, "Math": 8, "English": 4, "Engineering": 3}

# --- Contacts & Social Media ---
emergency_contact = ("Mom", "Kia McDaniel", "301-263-5223")
home_address = ("1011 Bohac Ln", "Accokeek", "MD", 2)

instagram_info = ("Instagram", "@sirrche", 312)
twitter_info = ("Twitter", "@chickencheesewraps", 127)

contact_dict = {
    "Mom": "301-263-5223",
    "Brother": "202-644-3386",
    "Academic Advisor": "336-334-5000"
}

# --- Personal Info ---
user_birthdate = ("Birthday", 11, 15, 2007)

current_skills = {"Python", "Sculpture", "Gardening", "Time management", "Ge"}
skills_learn = {"Coding", "Data structures", "Git", "Web design", "Types"}
career_interests = {"Software development", "Web development", "Data science", "Game development"}
hobbies = {"Gaming", "Gardening", "Reading", "Basketball", "Music"}
entertainment = {"One Piece", "AOT", "South Park", "Family Guy", "Naruto"}

# === Calculations ===
total_credits = sum(credit_hours)
avg_gpa = sum(gpa_history) / len(gpa_history)
credit_amount = len(course_list)
weekly_study_time = sum(study_dict.values())
academic_investment = budget_dict["Books"] / weekly_study_time
total_budget = sum(budget_dict.values())
food_budget = budget_dict["Food"] / 30
annual_budget = total_budget * 12
follower_count = twitter_info[2] + instagram_info[2]
current_skills_count = len(current_skills)
learning_skills_count = len(skills_learn)
contact_size = len(contact_dict)
entertainment_count = len(entertainment)
academic_assessment = len(hobbies)

# === OUTPUT ===
print("================================================================")
print("              PERSONAL ACADEMIC & LIFE PORTFOLIO")
print("================================================================")
print(f"Student: {full_name} | Email: {student_email}")
print(f"From: {hometown} | Graduating: {graduation}")
print(f"Major: {major}")
print("")
print("=== ACADEMIC PROFILE ===")
print(f"Current Semester: {total_credits} credits across {credit_amount} courses")
print(f"Cumulative GPA: {avg_gpa:.2f}")
print(f"Weekly Study Time: {weekly_study_time} hours")
print(f"Academic Investment: \n${academic_investment:.1f} per study hour")
print("")
print("Current Courses:")
for course in course_list:
    print(f"{course} - {credit_dict[course]} credits - {professors_dict[course]} - {rooms_dict[course]}")
print("")
print("=== PERSONAL DEVELOPMENT ===")
print(f"Current Skills: {current_skills}")
print(f"Learning Goals: {skills_learn}")
print(f"Career Interests: {career_interests}")
print(f"Skills Currently Have: {current_skills_count}")
print(f"Skills Want to Learn: {learning_skills_count}")
print("")
print("=== FINANCIAL OVERVIEW ===")
print(f"Monthly Budget: ${total_budget}")
print(f"Food: ${budget_dict['Food']} (${food_budget:.1f}/day)")
print(f"Entertainment: ${budget_dict['Entertainment']}")
print(f"Books: ${budget_dict['Books']}")
print(f"Transportation: ${budget_dict['Transportation']}")
print(f"Annual Projection: ${annual_budget}")
print("")
print("=== CONNECTIONS & CONTACTS ===")
print(f"Emergency Contact: {emergency_contact[1]} ({emergency_contact[0]}) - {emergency_contact[2]}")
print(f"Home Address: {home_address[0]}, {home_address[1]}, {home_address[2]} {home_address[3]}")
print(f"Social Media Presence: {follower_count} followers across 2 platforms")
print(f"Key Contacts: {contact_size} people in directory")
print("")
print("=== LIFE STATISTICS ===")
print(f"Total Courses Completed: {len(completed_courses)}")
print(f"Current Academic Load: {weekly_study_time + total_credits} weekly commitments")
print(f"Entertainment Backlog: {entertainment_count} items")
print(f"Current Hobbies: {academic_assessment} activities")
print("================================================================")
