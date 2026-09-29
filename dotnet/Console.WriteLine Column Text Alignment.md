
```c# title:"String Interpolation"
// Define some sample data
string[] names = { "Alice", "Bob", "Charlie" };
string[] depts = { "Engineering", "HR", "Marketing" };
int[] ids = { 101, 4, 12055 };

// Print the Header (Left-align Name/Dept by 15 chars, Right-align ID by 8 chars)
Console.WriteLine($"{"Name",-15} | {"Department",-15} | {"ID",8}");
Console.WriteLine(new string('-', 46)); // Divider line

// Print the Rows
for (int i = 0; i < names.Length; i++){
    Console.WriteLine($"{names[i],-15} | {depts[i],-15} | {ids[i],8}");
}

```


```c# title:"Composite Formatting"
// Syntax: {index, alignment}
Console.WriteLine("{0,-15} | {1,-15} | {2,8}", "Name", "Department", "ID");
Console.WriteLine(new string('-', 46));

for (int i = 0; i < names.Length; i++){
    Console.WriteLine("{0,-15} | {1,-15} | {2,8}", names[i], depts[i], ids[i]);
}
```