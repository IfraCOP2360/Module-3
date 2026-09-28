# Module-3
Console.WriteLine ("Enter the number of pandas: ");
String input1 = Console.ReadLine();
int numPandas = Convert.ToInt32(input1);

Console.WriteLine ("Number of pandas: " + numPandas);     // Number of pandas: 1
  Panda p = new Panda { Name = "mia" };
  Console.WriteLine ("My panda name is " + p.ToString());
   // My panda name is Petey

for (int i = 0; i < numPandas; i++)
{
  Console.WriteLine ("Enter the name of panda " + (i + 1) + ": ");
  String name = Console.ReadLine();
    p.Name = name;

  Console.Write ("Panda {0}", i + 1);
  Console.WriteLine (" name: " + p.ToString());     // My panda name is Petey
 
}


public class Panda
{
  public string Name;
  public override string ToString() { return Name; }
}

