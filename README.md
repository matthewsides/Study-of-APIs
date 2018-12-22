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


Images below detail the conceptual designs for the games UI, opting to garner inspiration from franchises such as Halo and 


The first design illustrates a menu in which the camera would be in constant motion,looping around and following a mapped path in which the start and end would meet, rather than manual transformation forcing the camera to a specific position. The reason behind opting to use a connected path rather than a line which upon completion teleports the camera back to the start is to give it a smoother transistion.


This wireframe is the second iteration of the menu, used to diversify the options in regards to menu layout and functionality.
 
### API and Development enviroment for an Application 
For the purpose of this project, the API that was decided upon was the scripting API provided by Unity (Unity,2018). Unitys Scripting API pertaining to various API's (UnityEditor, UnityEngine, Unity) grouped by namespaces. The central API being used for the development is the Unity Engine, enabling access to features that can support the development and formulation of scripts.

Following the choice of API leads into the choice of the development enviroment, as the API is relative to the Unity engine it only makes sense to use Unity. The inconnectivity of the API and development enviroment was the main drive behind utilising both.In addition to Unitys intuitive interface, access to numerous turtorials and vast amount of tools and API's (free scripts) avaliable. Although Unity was not the only development enviroment taken into consideration with the Unreal engine,a complete suite of tools developed by Epic Games used primarily for the development of applications, also a possibility (Unreal Engine, 2004-2018). Though due to the Unreal Engines sophisticated interface that doesn’t facilitate ease of use, lack of turtorials, Unitys improved graphics and lighting system  brought about through Unitys 2018f update and own experience using Unity, was eventually decided upon.

### Implementation

An iteration of the game was developed, as seen below.This prototype includes object collision, movement and a prototype camera.

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/PrismaTP.png?raw=true "Optional Title")

In relation to Unitys Scripting API the camera system utilises quaternion values and euler angles to represent the rotation and return the orientation (rigidbody) of the camera clamping the view based on private predefined values.

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/CameraClampEX.png?raw=true "Optional Title")

The access modifers also function in conjunction with Unitys software, meaning that all variables identified as Public can be accessed via the inspector, allowing the clamp angle, sensitivity, speed, etc. to be changed without the requirement of going into Visual studios.

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/PrismaIV.png?=50x50)

Unity also includes pre-set colliders and rigid bodys, which were applied in order to simulate physics and collision, ensuring that the player did not Phase through Objects. The collider itself includes its own pre-set classess and is under the Unity Engine API. Although in this aspect no code has currently been used for collision, opting to use Unitys in-built collision detection system as a placeholder until further development.

![Alt text](https://github.com/matthewsides/Study-of-APIs/blob/master/PrismaEV.png?raw=true "Optional Title")









Biblography

Beal. Vangie, (No date). API - application program interface. Available at: https://www.webopedia.com/TERM/A/API.html [Accessed: 17/11/2018].

Cooper. Jackason, (2017). How to generate a random number. Available at:https://www.pythoncentral.io/how-to-generate-a-random-number-in-python/ [Accessed: 19/11/2018].

Cplusplus.com, (no dtae). Function Rand. Available at: http://www.cplusplus.com/reference/cstdlib/rand/ {Accessed: 19/11/2018].

Oracle.com (1997, 2018).Class Random. Available at: https://docs.oracle.com/javase/8/docs/api/java/util/Random.html [Accessed: 19/11/2018].

Pearlman. Shana, (2016). What are APIs and how do APIs work? Available at: https://blogs.mulesoft.com/biz/tech-ramblings-biz/what-are-apis-how-do-apis-work/ [Accessed: 17/11/2018].

Stackoverflow (2018). If I don't specify srand(), what seed does rand() use? Available at: https://stackoverflow.com/questions/14251452/if-i-dont-specify-srand-what-seed-does-rand-use [Accessed: 20/11/2018]

Tutorials Point (No date). Java.util.Random Class. Availabale at: https://www.tutorialspoint.com/java/util/java_util_random.htm [Accessed: 18/11/2018].

Unity Documentation, (2018). Scripting API.  Available at: https://docs.unity3d.com/ScriptReference/index.html [Accessed: 20/11/2018].

Unreal Engine, (2004-2018).About Unreal Engine 4. Available at: https://www.unrealengine.com/en-US/features [Accessed: 17/11/2018].

