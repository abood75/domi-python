# domi-python
training
class student(object) :
      def __init__(self,name,age,gender,level,grades=None) :
         self.name = name
         self.age = age
         self.gender = gender
         self.level = level
         self.grades =grades
      def setGrade(self, course, grade):
          self.grades[course] = grade
          getgrade(self, course) 
          return self.grades[course]
      def gpagrade(self):
          return sum(self.grades.values())/len(self.grades)
        
salem=student("salem",22,"male",4,{"math":5.6,"quran":3.5})
print(salem.gpagrade())
