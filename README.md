# How to get Godot print and debug to work with Visual Studio 2022 (C#)
How to achieve a "hacky" way to get print messages and be able to debug using Visual Studio 2022 and Godot (using C#)

For those that need to work with Visual Studio 2022 and Godot, there is not an easy way to get the debug and GD.Print messages working for C#.

To make this solution work, just copy the GD.cs file and put it anywhere in your project. [https://github.com/DanTrz/Godot-GD.Print-and-Error-in-Visual-Studio-2022/blob/main/GD.cs]

It will get calls from Godot GD.Print and other methods and will forward it to the Debuger in Visual Studio so you can see themm in the console. In short, this will pipe GD.Print functions to the Visual Studio 2022 output window.

The original solution I found was uploaded by SilentPenguin here: https://gist.github.com/SilentPenguin/bf24eb348c9d00c34605d1cc54318be7

My version has modifications to try and make it a bit simpler and potentially faster, with less impact. There is some minimal performance impact, and this is not really recommended unless you really need to debug and workg with Visual Studio 2022 and require a way to check Godot GD.Print or similar methods. 

First, you need to make sure Visual Studio is correctly setup. If you need help, this link gives you the basic information required: https://www.reddit.com/r/GodotCSharp/comments/xgpqfh/oc_rundebug_godot4_c_projects_from_visual_studio/?onetap_auto=true 

