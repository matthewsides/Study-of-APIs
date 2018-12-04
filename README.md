# Study-of-APIs

## API
An Application Programming Interface (API) is a specification intended to be used as an interface by software components to communicate with each other. An API may include specifications for pre-defined subroutines,classes,communication protocols, variables and is an integral tool for the development of software. Essentially because APIs are building blocks for potentional powerful solution capabilities, meaning an API for instance pertianing to the function of adding and subtracting numbers can be applied and imported into software unrelated allowing cross communication between programs and meaning that said programmers no longer have to bother with the logisitics behind or implementation of such a function. However this is dependant on whether the API relates to the specification, functionality and design of the software,thus highlighting the importance of evaluating whether an API is suitable to said scenario. The example of an API that can subtract and add numbers would be usable if for instance the program or application being created was a calculator. 

### Examples of APIs:
Java API

Google Maps API

Flash Player API


##  Relationship between an API and a SDK
An API as stated under the API heading, is a series of related methods (a specification) intended to be used for a specific purpose and as an interface by software components to communicate with each other. Whilst an SDK is just a sample of how you would interact with said APIs, Thus the relationship between an API and SDK can be seen through theses definitions as an SDK is used as a buffer to access collate and communicate with the APIs. Through using this method (SDK) it essentially blocks access to the code thus improving the security measures as the API cannot be tampered with. Whilst if the Print function (API) in python (SDK) is taken as an example it allows you to set the parameters of say a print method that are pre-defined, meaning that there is no thought process required in how to achieve or do that. Although because the parameters and functions are pre-determined, it may be seen as both an advantage and limitation as what is feasible is decided by the programmer of that API.

## Platform use of API's and Comparision 

API's have a broad range, meaning that there are multiple API's for numerous tasks.However API's are generally native, meaning that the API is language specific and the code is directly executing abstract functionality. Although an API can also define a protocol for accessing that same functionality, as stated each language generally has there own API with pre-defined methods to meet a specific purpose. The way inwhich the same API functions across each platform/language differs, this is fudementally due to the type of programming, structure, intended purpose when formulated and overall functionality. 

The ideology behind for instance an 'random number generator API' is to make it easier (manipulate software) to produce random numbers or create the illusion of numbers generating in a random fashion, this is the ideology regardless of the language. 

In C++ the 'rng API', a programming API, returns a pseudo-random integral number in the range between 0 and RAND_MAX. The 'random number generator API' uses a seed to generate the series, which should be initialized to some distinctive value using the function srand(), generating the pseudo-random numbers using the rand() function. If srand() is not called, the rand() seed is set and interpreted as if srand(1) were called at the program start. Any other value for seed sets the generator to a different starting point.

Incontrast to C++ 'rng API',Javas terminology (labelling) of functions is different with 'rand()'  called 'Random()' and 'Srand' called Random(long seed),etc.Although there is no distinction in the proccess or ideology behind the functions a number is still generated ('Random()') and required to be seeded prior to generation.

Python however functions different to both Java and C++ with regards to the proccess used for generating a random number in addition to the evident change in terminology and libary imported (Python uses 'random',C++ uses '' and Java '').The generation of a random number rather then segrgated into seperate lines is primary initialised or set on one line, with Python requiring its variables types (string,int,float,etc.) to be defined manually   As python requires the variable type to be defined,

the initialisation of the range in which the numbers 










The issues that stem from using the rng API is that the RAND_MAX function has a minimum specified value of 32,767. Portable code cannot assume that the range is any larger than this, so portable code is very limited in the random numbers that can be predictably generated. 

Moreover since rand is not required to conform to any standard distribution, the base random number generator is expected to return values in a uniform distribution. Thus meaning that every number in the range is equally likely to be returned for any given request. Even when rand claims a uniform distribution, it may not be a terribly good distribution, which greatly affects any attempts to adjust the range.

## Security issues pertaining to API's











