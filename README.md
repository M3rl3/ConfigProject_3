# Configuration & Deployment - project03

Project repository for GDP - 2022. (Configuration & Deployment - INFO-6025)

<h3> Build Instructions: </h3>
<ul>
<li>Solutuion has one project which is automatically the default project.
<li>Built in Visual Studio 17 (2022). Retarget solution if necessary.
</ul>

<h3>MSBuild:</h3>
<ul>
<li>The MSBuild script can be found in "$(ProjectDir)ConfigProject_3.vcxproj".
<li>The project is designed to only work in Debug mode, building on Release will build the project but not generate any files.
<li>MSBuild will generate the executable and all the dependencies under "c:\cnd\".
<li>A zip file is also generated in the same directory which includes all the files needed to run the project.
<li>The MSBuild command used to build and generate said files is included below.
<li>Here, "./" will be the working directory followed by the solution directory for the project.
</ul>

```
MSBuild.exe .\ConfigProject_3\ -t:project_03 -property:Platform=x64 -property:Configuration=Debug
```

<h3>Gameplay and related: </h3>
The setting of this game potrays a long dark highway dimly lit by street lamps on each side.
</br>A lone tesla cybertruck has the task of traversing said landscape in the dead of the night. 

<h3>Controls:</h3>
<ul>
<li>The user can control the truck by pressing the 'F' key.
<li>User can iterate through objects in the scene by pressing 'O'. This also locks the camera on the object being pointed to.
<li>NUM1 focuses the camera on the origin(0,0,0) of the scene, NUM2 focuses the camera on the next mesh while NUM3 focuses on the previous.
<li>The name of the object in question is outputed to the titlebar of the window.
<li>The camera can be accessed at any point by pressing the 'C' key.
<li>The 'X' key can be used to turn all models in the scene into wireframe mode.
</ul>

A combination of W,A,S,D,Q,E keys can be used to move the models or the camera when in their respective modes.
