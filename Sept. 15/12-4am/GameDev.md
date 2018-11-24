## Game Dev: Intro to Unity
### Presenter: Adam Leung

**Target Audience:** 
- Programmers who would like to learn about the basics of using Unity to make games

**Suggested Prerequisites:** 
- Basic programing knowledge (variables, conditional statements, while and for loops)
- An interest in making video games 
- A laptop with Unity installed

**Workshop Goals:**

Give learners the tools and knowledge to create a working game in Unity. 

**Description:**

Learn how Unity's editor is structured, how Unity projects are structured, how Unity's scripting is structured, and how to use all of those together to create an idea. We'll go through a common sense approach of how to execute on the idea of making a 2D platformer, and how one can go about coding, debugging, and iterating on that idea.

**Content Breakdown:**
- Introduction
    - What is a game engine/Unity
    - Why choose Unity
- Unity Introduction
    - Creating a project
    - Explaining each part of the UI
    - Scene View
         - Game View
         - Hierarchy
         - Inspector
         - Project
         - Console
         - Play, pause, next frame buttons
- Basic programming
    - Comments
    - Debug.Log()
    - Data types
         - Int
         - Bool
        - Float
        - String
    - If statements
    - Boolean operators
- Importing assets
    - Adding new assets to project
    - Adding sprites to scene
- Basic Unity programming
    - Concept of components
    - Start(), Update()
    - Accessing and changing components
    - Getting player input via Input.Get...
- Adding physics and basic controls
    - Rigidbody & Collider components
    - Public variables
    - Move character left and right
    - Make character jump
- Collisions and powerups 
    - OnCollisionEnter() checks
    - Accessing other gameobject’s components
    - Changing speed
- Closing/Q&A
    - What to build upon, look into
    - Outro, links to code and more

**Resources**
- [Code](https://github.com/Centribo/unity-starter-tutorial)
- [Assets](http://www.centribo.com/unityAssets.zip)

**[Slides](http://bit.ly/UWGDCUnity101)**

--- 

**Key Notes:**
* Game Engines
    * Game engines are like any other tool or framework
    * Choose the right tool for the job, choose the right game engine for your game

* Unity Projects
    * Just a folder structure
    * “Assets” is where everything you want in your game to go


* Unity UI
    * Scene View = The behind the scenes developer’s view
    * Game View = What the player who is playing your game sees
    * Hierarchy = What objects and entities are in your game right now
    * Inspector = Specific details and properties of a certain object
    * Project = File browser to see all the assets in your game
    * Console = Debugging console, useful for printing errors/information to


* Scripting/Programming
    * Everything exists as a “GameObject”
    * Every GameObject has components that add functionality or behaviour to it
    * Almost always, you are adding components to GameObject
    * Every GameObject will have at least a transform component that tells Unity where it exists in 3D space, how it is rotated, and how it is scaled
    * Input
        * In Unity: Edit -> Project Settings -> Input
        * Access inputs via https://docs.unity3d.com/ScriptReference/Input.html in code
        * For example: Input.GetButtonDown("Fire1")
    * For everything else: https://docs.unity3d.com/ScriptReference/
