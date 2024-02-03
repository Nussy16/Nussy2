# Python program that demonstrates the use of lists, tuples, and sets to organize and analyze a dataset

students_data = [
    {'name': 'Amatullah', 'age': 20, 'major': 'Computer '},
    {'name': 'Ihsan', 'age': 22, 'major': 'Engineering'},
    {'name': 'Rahma', 'age': 21, 'major': 'Mathematics'},
    {'name': 'Maryam', 'age': 20, 'major': 'Physics'}
]

# List of names
names_list = [student['name'] for student in students_data]

# Tuple of unique majors
majors_tuple = tuple({student['major'] for student in students_data})

# Set of unique ages
ages_set = {student['age'] for student in students_data}

# Analysis
num_students = len(students_data)
num_unique_names = len(set(names_list))
num_unique_majors = len(majors_tuple)
avg_age = sum(ages_set) / len(ages_set)

# Output
print("Dataset Analysis:")
print(f"Number of students: {num_students}")
print(f"Number of unique names: {num_unique_names}")
print(f"Number of unique majors: {num_unique_majors}")
print(f"Average age of students: {avg_age:.2f}")

# In this program

#I have a sample dataset students_data, which contains information about students.
# I used list comprehension to create a list of names (names_list), then used set comprehension to create a tuple of unique majors (majors_tuple).
# I use set comprehension to create a set of unique ages (ages_set) and performed some basic analysis on the dataset, such as counting the number of students, the number of unique names, the number of unique majors, and calculating the average age.
# Lastly, the result of the analysis was printed.￼Enter
