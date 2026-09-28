# Module-3
// Prompt the user to enter the number of students
Console.WriteLine ("Enter the number of students: ");
String input1 = Console.ReadLine();
int numStudents = Convert.ToInt32(input1);

Console.WriteLine ("Number of Students: " + numStudents);     // Number of Students: 1
// Create a new Student object
  Student s = new Student { Name = " " };
// Loop through the number of students and prompt for their names
for (int i = 1; i <= numStudents; i++)
{
  Console.WriteLine ("Enter the name of Student " + (i) + ": ");
  String name = Console.ReadLine();
    s.Name = name;
// Display the student's name using the overridden ToString() method
  Console.WriteLine ("Student {0} name: {1}", i, s.ToString());
}

// Create a new Student object and set its name
public class Student
{
  public string Name;
  // Override the ToString() method to return the student's name
  public override string ToString() { return Name; }
}
