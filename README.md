# Module-3
int x = 1;
string s = x.ToString();     // s is "1"

Panda p = new Panda { Name = "Petey" };
Console.WriteLine ("My panda name is " + p.ToString());     // My panda name is Petey

public class Panda
{
  public string Name;
  public override string ToString() { return Name; }
}
