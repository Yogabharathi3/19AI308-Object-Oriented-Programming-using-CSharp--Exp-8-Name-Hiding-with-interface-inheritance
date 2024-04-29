# 19AI308-Object-Oriented-Programming-using-CSharp--Exp-8-Name-Hiding-with-interface-inheritance

# AIM:

To implement name hiding with interface inheritance. Aim is to create an interface IMario with a method Ability(). 
Implement this interface in a class Mario and override the Ability() method also to create another class SuperMario that inherits from Mario 
and hides the Ability() method using the new keyword.

# PROGRAM:
```
Developed by:Yogabharathi S
Register number:212222230179
```
```
using System;
public interface IMario
{
    void Ability();

}
class Mario:IMario{
    public virtual void Ability()
    {
        Console.WriteLine("Mario's Ability:Normal Dancing");
    }
}  
class SuperMario:Mario
{
    public new void Ability()
    {
        Console.WriteLine("Mario's Ability:Super Dancing");
    }
}
class Program
{
    static void Main(string[]args)
    {
        IMario mario=new Mario();
        SuperMario superMario=new SuperMario();
        mario.Ability();
        superMario.Ability();

    }
}
```

# OUTPUT:

![Screenshot 2024-04-27 115317](https://github.com/22008686/19AI308-Object-Oriented-Programming-using-CSharp--Exp-8-Name-Hiding-with-interface-inheritance/assets/118916413/51ccc631-e0fa-4069-9138-fb23b069376f)

# RESULT:

Thus, the program has been executed successfully.
