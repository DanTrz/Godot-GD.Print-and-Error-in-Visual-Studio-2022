# How to get Godot print and debug to work with Visual Studio 2022 (C#)
How to achieve a "hacky" way to get print messages and be able to debug using Visual Studio 2022 and Godot (using C#)


For those that need to work with Visual Studio 2022 and Godot, there is not an easy way to get the debug and GD.Print messages working for C#.

To make this solution work, just copy the GD.cs file and put it anywhere in your project. It will get calls from Godot GD.Print and other methods and will forward it to the Debuger in Visual Studio so you can see themm in the console.

There is some minimal performance impact, and this is not really recommended unless you really need to debug and workg with Visual Studio 2022 and require a way to check Godot GD.Print or similar methods. 
