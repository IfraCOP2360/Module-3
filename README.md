# Module-3
Console.WriteLine ("Enter the number of pandas: ");
String input1 = Console.ReadLine();
int numPandas = Convert.ToInt32(input1);

Console.WriteLine ("Number of pandas: " + numPandas);     // Number of pandas: 1
  Panda p = new Panda { Name = " " };

for (int i = 1; i <= numPandas; i++)
{
  Console.WriteLine ("Enter the name of panda " + (i) + ": ");
  String name = Console.ReadLine();
    p.Name = name;

  Console.WriteLine ("Panda {0} name: {1}", i, p.ToString());
}


public class Panda
{
  public string Name;
  public override string ToString() { return Name; }
}
