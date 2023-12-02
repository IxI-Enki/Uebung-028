# Uebung-028  -- Turmrechner
<!--
## Lernziele:

## Aufgabenstellung:

### Beispiel:
### Beispielausgabe:

#### Hinweis:

-------------------------------
## *Zusatzaufgabe:*



-->
-------------------------------
# **SPOILER**

```c#
using System;
namespace Turmrechner
{
  internal class Program
  {
    static void Main()
    {
      string userInput;
      int userInteger, number;

      Console.Write("\n        Pyramidenrechner       " +
                    "\n================================");
      do
      {
        Console.Write("\n Geben Sie eine ganze Zahl ein." +
                      "\n ");
        userInput = Console.ReadLine();
        int.TryParse(userInput, out userInteger);

        number = userInteger;
        if (userInteger != 0)
        {
          for (int i = 2; i < 10; i++)
          {
            Console.Write($"\n {number} * {i} = {number * i}");
            number = number * i;
          }
          for (int i = 2; i < 10; i++)
          {
            Console.Write($"\n {number} / {i} = {number / i}");
            number = number / i;
          }
        }
      } while (userInteger != 0);

      
      Console.Write("\nZum Beenden bitte Eingabetaste drücken ...");
      Console.ReadLine();
      Console.Clear();
    }
  }
}
```
