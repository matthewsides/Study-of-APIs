# Study-of-APIs

## API
An Application Programming Interface (API), is a specification intended to be used as an interface by software components to communicate with each other. An API may include specifications for pre-defined subroutines,classes,communication protocols, variables and is an integral tool for the development of software (Beal, No date). Essentially, APIs are building blocks for potential powerful solution capabilities, meaning an API for instance pertaining to the function of adding and subtracting numbers can be applied and imported into software unrelated allowing cross communication between programs and meaning that said programmers no longer have to bother with the logisitics behind or implementation of such a function. However, this is dependant on whether the API relates to the specification, functionality and design of the software,thus highlighting the importance of evaluating whether an API is suitable to said scenario. The example of an API that can subtract and add numbers would be usable if for instance the program or application being created was a calculator (Peralman, 2016). 

### Examples of APIs:
Java API

Google Maps API

Flash Player API

##  Relationship between an API and a SDK
An API as stated under the API heading, is a series of related methods (a specification) intended to be used for a specific purpose and as an interface by software components to communicate with each other. Whilst an SDK is just a sample of how you would interact with said APIs. Thus the relationship between an API and SDK can be seen through these definitions, as an SDK is used as a buffer to access collate and communicate with the APIs. Through using this method (SDK) it essentially blocks access to the code, thus improving the security measures as the API cannot be tampered with. Whilst, if the print function (API) in python (SDK) is taken as an example, it allows you to set the parameters of say a print method that are pre-defined, meaning that there is no thought process required in how to achieve or do that. Although because the parameters and functions are pre-determined, it may be seen as both an advantage and limitation, as what is feasible is decided by the programmer of that API.

## Platform use of API's and Comparision 
API's have a broad range, meaning that there are multiple API's for numerous tasks. However, API's are generally native, meaning that the API is language specific and the code is directly executing abstract functionality. Although an API can also define a protocol for accessing that same functionality, as stated each language generally has their own API with pre-defined methods to meet a specific purpose. The way in which the same API functions across each platform/language differs, this is fundamentally due to the type of programming, structure, intended purpose when formulated and overall functionality. 

The ideology behind, for instance a 'random number generator API', is to make it easier (manipulate software) to produce random numbers or create the illusion of numbers generating in a random fashion, this is the ideology regardless of the language (Cooper 2017). 

In C++ the 'cstdlib API', a programming API, returns a pseudo-random integral number in the range between 0 and RAND_MAX (Cplusplus.com, no date). The 'cstdlib API' uses a seed to generate the series, which should be initialised to some distinctive value using the function ‘srand()’, generating the pseudo-random numbers using the ‘rand()’ function. If srand() is not called, the rand() seed is set and interpreted as if srand(1) were called at the program start. Any other value for the seed sets the generator to a different starting point.

In contrast to C++ 'cstdlib API', Java's terminology (labelling) of functions is different, with 'rand()'  called 'Random()' and 'Srand' called ‘Random(long seed)’, etc (Oracle.com (1997,2018. Although there is no distinction in the process or ideology behind the functions, a number is still generated ('Random ()') and required to be seeded prior to generation (Tutorials Point No date).

Python however functions differently to both Java and C++ with regards to the process used for generating a random number. In addition to the evident change in terminology and library imported (Python uses 'random’, C++ uses 'cstdlib' and Java the 'java.util.Random class'), the generation of a random number rather than spread across separate lines, is primarily initialised or set on one line. Whilst Python interprets the type, meaning that it is not required to explicitly declare the data types of variables, in comparison to Java's and C++ approach of requiring the scope to be defined inside a type definition before generation. Though Python is still capable of forcing the type if necessary. Moreover, unlike C++ or Java that uses two separate functions that sets a seed (start state) along with a pre-defined max integer that work in correlation, Python defines a range stored in brackets on the same line the random function is called on.


## Prisma
Prisma is a conceptual third person shooter or action game, formulated around the ideology that current third person action or shooters have become too reliant on cover systems and hold or are plagued with a lack off depth. The scope of this application encompasses, primarily though not limited too, those whom enjoy third person games. In particular those relating to the shooter and action genres respectively. Moreover, based on the Pan European Game Information (PEGI) Rating system and due to the core nature of the game being a third person action or shooter presenting visible violence, the game is likely to fall under the catagory of a 12 or 16 plus game, meaning that the audience will be restricted to 12 or 16 and above.

With regards to platform or system compatability, the current plans for the game entail developing it to be playable only on PC compatible computers as a desktop application.This is primarily due to time contraints, although the 'Prisma' will be controller compatible, meaning that the game can be played with a controller in addition to the keyboard and mouse, catering to those who usually play games via console.


Images below detail the conceptual designs for the games UI, opting to garner inspiration from the franchise Halo, a critically acclaimed video game series. 

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/Menu_Alternate.png?raw=true "Optional Title")

The first design (shown above) illustrates a menu in which the camera would be in constant motion,looping around and following a mapped path in which the start and end would meet, rather than manual transformation forcing the camera to a specific position. The reason behind opting to use a connected path rather than a line which upon completion teleports the camera back to the start, is to give it a smoother transistion.

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/Menu.png?raw=true "Optional Title")

This wireframe (shown above) is the second iteration of the menu, used to diversify the options in regards to menu layout and functionality.
 
### API and Development enviroment for an Application 
For the purpose of this project, the API that was decided upon was the scripting API provided by Unity (Unity,2018). Unity's Scripting API pertaining to various API's (UnityEditor, UnityEngine, Unity) grouped by namespaces. The central API being used for the development is the Unity Engine, enabling access to features that can support the development and formulation of scripts.

Following the choice of API, leads into the choice of the development enviroment, as the API is relative to the Unity engine it only makes sense to use Unity. The inconnectivity of the API and development enviroment was the main drive behind utilising both. In addition to Unitys intuitive interface, access to numerous turtorials and vast amount of tools and API's (free scripts) are avaliable. Although Unity was not the only development environment taken into consideration, with the Unreal Engine, a complete suite of tools developed by Epic Games used primarily for the development of applications, also a possibility (Unreal Engine, 2004-2018). Though due to the Unreal Engines sophisticated interface, that does not facilitate ease of use and lack of turtorials, Unitys improved graphics and lighting system,  brought about through Unitys 2018f update, and own experience using Unity, Unity was eventually decided upon.

### Implementation

An iteration of the game was developed, as seen below. This prototype includes object collision, movement and a prototype camera.

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/PrismaTP.png?raw=true "Optional Title")

In relation to Unitys Scripting API, the camera system utilises quaternion values and euler angles to represent the rotation and return the orientation (rigidbody) of the camera clamping the view based on private predefined values.

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/CameraClampEX.png?raw=true "Optional Title")

The access modifers also function in conjunction with Unity's software, meaning that all variables identified as Public can be accessed via the inspector, allowing the clamp angle, sensitivity, speed, etc. to be changed without the requirement of going into visual studios.

<img src="https://github.com/matthewsides/Study-of-APIs/blob/master/PrismaIV.png" width="200" height="400">

Further delving into the ideology behind the camera system, an empty game object is attached to the playerobject, this is used as reference for the camera in regards to what it should follow. The 'Transform target = CameraFollowObj.transform;' line sets the object to follow, whilst 'float step = CameraMoveSpeed * Time.deltaTime;' and 'transform.position = Vector3.MoveTowards(transform.position, target.position, step);' moves the camera to the game object that is set as the target.


While the collision aspect of the camera applies an occolusion detection system that zooms the camera in upon camera obstruction to ensure that the player character is always in view. Another aspect or element that is set to be implemented is upon collision with an object the mesh shall turn invisible, this should eliminate object clipping and is a mechanic inspired by a feature in the batman game franchise.

Unity also includes pre-set colliders and rigid bodys, which were applied in order to simulate physics and collision, ensuring that the player did not Phase through Objects. The collider itself includes its own pre-set classess and is under the Unity Engine API. Although in this aspect no code has currently been used for collision, opting to use Unitys in-built collision detection system as a placeholder until further development.

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/PrismaEV.png?raw=true "Optional Title")

The animations and objects were rigged to humanoid and intergrated through using Unity's Animator, which is an inbuilt tool and apart of Unity's Engine API, calling the animator in visual studios to return a value depending on whether a key has been pressed using a trigger (event) system.

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/PrismaAC.png?raw=true "Optional Title")

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/PrismaAR.png?raw=true "Optional Title")

### Testing

White Box - This form of testing refers to testing the functionality being aware of the internal structure. This was used to determine any issues in regards to functionality and allowed for fixes.

|Test Reference No.|Test Description | Type of Test | Expected Result | Observed Result |
|---|---------------|--------------|-----------------|-----------------|
|1. | API Imported correctly| White Box |The Scripting API (Unity Engine) defined at the start of the code should not display any errors in either the console or visual studios C# code upon using its features (classes and functions). | Passed - The API was successfully imported and its features functional. |
|2A. | Camera is assigned and follows a game object| White Box | Camera should move towards the assigned object regardless of its position. | Failed - The camera appears to position itself in a position not relative to the game object, remaining static.
|2B.| Camera is assigned and follows a game object | White Box |Camera should position itself in view of the game object and follow it. | Passed - The issue stemmed from the empty object which is used as the empty object not being in the right position in the Hierachy and in the scene view. |
|3.| Key press triggers action | White Box | Upon pressing a key which is pre-mapped the player should show output | Passed - Upon pressing the pre-mapped button, in this instance 'W', the player did show output, displaying a run animation and moving forward. |
|4. | Camera collision detection | White Box | The camera should collide with objects avoiding clipping. | Passed - The camera upon contact with other objects pushes the camera away from the object, though there is still slight clipping which in future can be rectified by hiding the mesh of certain or all objects upon contact. |
|5. |Camera occlusion detection | White Box | If the player object is out of the camera view the camera should zoom in towards the character, moving back to its original position when the camera is no longer obscured. | Passed - The camera upon losing sight of the character, attempts to move the camera closer to the player to ensure that the player view is not obscured, whilst the camera also zooms in upon collision with objects. |
|6A.| Player object pivots or rotates based on camera direction | White Box |The player model or object should turn based on the cameras rotation. | Failed - The player model did not rotate based on where the camera is looking. |
|6B.| Player object pivots or rotates based on camera direction | White Box | The player model should turn inconjunction to where the camera is facing. | Passed - This was fixed through setting the assigned player object to follow the same parameters or rotation set for the camera. |

Black Box - This testing relates to using user's whom know nothing about the internal structure of the code, with the functions being tested purely based on visual. 

|Tester: Luke Bruni|Test Reference No.|Test Description | Type of Test | Expected Result | Observed Result |
|------------------|--------|----------|---------|--------------------|------------------------|
|                  |1A.      | Camera  |  Black box | The camera should clearly show the player at all times and be able to follow and keep up with the player. | Failed - The camera followed the player with the player in view the majority of the time however, the camera failed to keep up upon continously running forward. |
|                  |1B.      | Camera | Black box | The camera should clearly show the player at all times and be able to follow and keep up with the player. | Passed - The camera was able to keep the player in clear view, following the player and keeping up with the player pacing. |
|                  |2.      | Player Movement-Forward | Black box | The player should move forward upon giving input. | Passed -  The player successfully moves foward after giving input. |
|                  |3A.     | Player rotation | Black box | The player should look and move based on where the camera is looking.| Failed - Though the player moved and looked based on the cameras direction, the player also followed the cameras rotation on the Y axis causing it to look unnatural.
|                  |3B.     | Player fixed rotation | Black box | The player should look and move based on where the camera is looking, with the player rotation fixed to the X axis.| Passed -  The player no longer follows and rotates with the camera upon looking up or down. |
|                  |4.      | Player Collision  | Black box | Player should not phase through objects | Passed - The player does not phase through objects upon contact. |



### Improvements
Following the  black and white box tests and anaylising the feedback, it was clear that there was an issue pertaining to player object rotation. Therefore it was devised to utilise the cameras pre-coded local rotation variable which returned the quaternion euler angles values based on the Y, X and Z axis, through attaching the same values the camera uses for rotation the player object was supposed to turn based on where the camera was looking. However, after this fix for the White box test carried out, the Black box tests carried out provided information seeming to show that although the issue of player rotation had been fixed, another issue relating to the player appeared. This issue related to the player model following the camera on the Y axis, meaning that if the player looked up the model would also change orientation, looking unnatural as the models feet were no longer connected to the floor which logically is not possible. Through freezing the players rotation on certain axis using the rigid body, appeared to fix the issue, though only temporary as a long term fix pertaining to locking the objects pivot on the Y axis has been identified and will be implemented in a future update. The reason behind why this current fix is ineligable, is due to the fact that the player object in future updates will need to be able to aim up with a gun to shoot targets in high places and this fix currently restricts this. Images of the issue can be seen below:

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/PrismaTestIssue.png?raw=true "Optional Title")

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/PrismaTestIssue2.png?raw=true "Optional Title")

A clamp was also considered and tested for the cameras Y axis making it impossible to look all the way up or down, thus making it impossible for this issue to occur. However as stated the camera would not be able to move freely thus restricting and constricting user view,whilst it was also possible to see the issue still. This fix was implemented and removed through the addition of the line; 'rotY = Mathf.Clamp(rotY, -clampAngle, clampAngle);', which can be seen in the image below:

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/PrismaRF.png?raw=true "Optional Title")


Further Improvements based on the white and black box testing,included fixing the cameras positioning which stemmed from the empty object, which is used as the empty object not being in the right position in the Hierachy and in the scene view. This entailed a simple alteration to the hierachy and re-positioning of the empty game object the camera is using as a basis to follow (using as a reference for the position and distance between the camera and player character).

Upon implementing these improvements and fixing the issues that were noted during both forms of testing, other changes that could be made to the current features in a future update pertains to hiding the mesh upon contact with the camera as a better way to avoid clipping and stop occolusion. Whilst using code to lock the players Y axis with the objects pivot and creating an offset to make the player rotation less smooth and more realistic (natural), are more changes that could be implemented in a future update to further improve on the current application (game).

### API's Used
Following the development of a prototype for the collective systems that will formulate a finished game and the potentional improvements outlined in the above paragraphs it is necessary to go into more detail into the API's used during development and in the final implementation. As stated in the API and development enviroment section Unity, the development enviroment used for the development of this prototype, provided a suite of tools,features and a plethora of API's,pre-set components and systems.For instance Unitys pre-defined physhics engine, which provided components that essentially handle the simulation of physics.It is also important to note that Unity has two physics engines one for 3D and another for 2D. 

In this instance the physics engine used was the 3D version, whilst the components provided by the physics engine utilised were the colliders, used to simulate collision and the rigidbody which dealt with gravity, though it can also be used to simulate other forces. Although it is plausible to control the physics through scripts giving an object different dynamics in this instance Unitys pre-sets were used. 

However there was scripting used for the movement of the player and camera, with the camera also using its own collider script. This was acheived through using Unitys Scripting API's or more specifically the Unity Engine API which is an API that includes a multitude of libraries with pre-written code that simply requires reference. The function called from the API UnityEngine to help alleviate development of the movement system was the transform function,every object contains a transform, which can be used to store and manipulate the position,rotation and scale of the object. Withregards to input GetKey or GetMouse classes of the UnityEngine were used and function through listening for an event or input with the state getting reset each frame as its placed within the Update (a native player loop). 

The camera movement also utlises the same scripting API and transform and input functions, however the proccess or calculation is done differently as a target is set for the camera to follow and placed as a child to the player in the hierarchy. Moreover Unitys Mathf library  is also used to clamp the value for the camera rotation using the clamp function inconjunction with quaternion which is used to represent the rotations of both the camera and player.

### How the application could be improved with the use of additional API's
The current iteration facilitates player input, movement,collision and gravity, however future builds in order to meet the design and direction of this project and improve upon the current build will include Main menu camera movement,AI and shooting. Bullet physics and 

## Biblography

Beal. Vangie, (No date). API - application program interface. Available at: https://www.webopedia.com/TERM/A/API.html [Accessed: 17/11/2018].

Cooper. Jackason, (2017). How to generate a random number. Available at:https://www.pythoncentral.io/how-to-generate-a-random-number-in-python/ [Accessed: 19/11/2018].

Cplusplus.com, (no date). Function Rand. Available at: http://www.cplusplus.com/reference/cstdlib/rand/ {Accessed: 19/11/2018].

Oracle.com (1997, 2018).Class Random. Available at: https://docs.oracle.com/javase/8/docs/api/java/util/Random.html [Accessed: 19/11/2018].

Pearlman. Shana, (2016). What are APIs and how do APIs work? Available at: https://blogs.mulesoft.com/biz/tech-ramblings-biz/what-are-apis-how-do-apis-work/ [Accessed: 17/11/2018].

Stackoverflow (2018). If I don't specify srand(), what seed does rand() use? Available at: https://stackoverflow.com/questions/14251452/if-i-dont-specify-srand-what-seed-does-rand-use [Accessed: 20/11/2018]

Tutorials Point (No date). Java.util.Random Class. Availabale at: https://www.tutorialspoint.com/java/util/java_util_random.htm [Accessed: 18/11/2018].

Unity Documentation, (2018). Scripting API.  Available at: https://docs.unity3d.com/ScriptReference/index.html [Accessed: 20/11/2018].

Unreal Engine, (2004-2018).About Unreal Engine 4. Available at: https://www.unrealengine.com/en-US/features [Accessed: 17/11/2018].

