# Inheritance-Students-
class Human:
    def __init__(self, age:int, grade: int):
        self.age = age
        self.grade = grade

class Transmission:
    def __init__(self, type:str = "automatic"):
        self.type = type

class Stats:
    def __init__(self, attendance:int, final_grade:int, done_homework:int):
        self.attendance = attendance
        self.final_grade = final_grade
        self.done_homework = done_homework

class Student(Stats):
    def __init__(self, transmission:Transmission):
        self.transmission = transmission


average_human = Human(10, 9)

average_grades = Stats(95, 92, 80)

mercedes = Human(average_grades, average_human)

print("Student:")
print(f"Info:\n\tAge:{average_human.age}\n\t Grade: {average_human.grade}\n\t")
print(f"Stats:\n\tAttendance:{average_grades.attendance}\n\tFinal Grade:{average_grades.final_grade}\n\tDone homework:{average_grades.done_homework}")
