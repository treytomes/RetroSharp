# RetroSharp

**RetroSharp** or **Retro#** is a C# library that makes learning to develop fun and easy by creating a development 
environment mimicking early development environments (retro), while maintaining the benefits of a modern language
like C#.

**RetroSharp** relies on [OpenTK](http://www.opentk.com/) for OpenGL rendering. It can be downloaded directly from
their site. A binary file (release from 2014-07-23) is also available in [Binaries folder](Binaries/OpenTK/Release) in this project. 
**RetroSharp** also relies on [OpenAL](https://www.openal.org/) for audio-output. An installation file for OpenAL
for Windows can also be found in the [Binaries folder](Binaries/OpenAL).

## How to begin

To create a retro-application using **RetroSharp**, you only need to reference the [RetroSharp](RetroSharp) library project and
derive your application from the [RetroApplication](RetroSharp/RetroApplication.cs) class. This class manages the retro environment,
including execution, character sets, sprites, rendering, console input/output, keyboard & mouse input, events, resources, audio,
hit-tests, drawing, file handling, etc., and it also manages the *OpenTK*, *OpenGL* and *OpenAL* libraries. Your application does 
not need to link to these libraries. The point of *RetroSharp* is to remove as much complexity of underlying libraries as 
possible, to make development quick, fun and easy and suitable for use for a first-time learner of programming.

## Templates

To make it easier to create a new project, there are two template projects available for you from the start:

| Template | Description |
|----------|-------------|
| [Character Template](Examples/CharacterTemplate) | The character template project sets up a retro console application for you. It's suitable for text-type applications. |
| [Raster Graphics Template](Examples/RasterGraphicsTemplate) | The raster graphics template project sets up a retro raster graphics application for you. It's suitable for applications where you need to need to draw on the screen. In raster graphics mode, you can still use console input/output if you choose to. |

To be able to use these templates from *Visual Studio*, you might have to export them first, once the solution has loaded.
Just select the template project in the *solution explorer* and select *Export Template...* from the *File* menu to export a
project as a *project template*. Once it has been exported as a *project template* it will be available as soon as you want to
create a new project, in the list of available templates.

## Examples

The solution includes a series of [examples](Examples) demonstrating how **RetroSharp** can be used. These [examples](Examples) 
are simple and aim to present a topic in a short and simple manner that is easy to read, understand, and reutilize. The 
[examples](Examples) are sorted into various categories, from very simple to more advanced, as shown below.

### Text and Strings

The examples sorted into the [Text and Strings](Examples/Text and Strings) category show how to input, process and output text in simple
console applications.

| Screen Shot | Project description |
|-------------|---------------------|
|![Hello World](Images/HelloWorld_20.png)| The [Hello World](Examples/Text and Strings/HelloWorld) project is probably the first project for many. It displays a "Hello World" message in a console application, just to show basic console output. |
|![Guess a number](Images/GuessANumber_20.png)| The [Guess a number](Examples/Text and Strings/GuessANumber) project lets the user guess a random number between 1 and 100. The application terminates when the user guesses the number correctly. |

### Arithmetics

The examples available in the [Arithmetics](Examples/Arithmetics) category show how to perform simple numerical calculations.

| Screen Shot | Project description |
|-------------|---------------------|
|![Simple Arithmetics](Images/SimpleArithmetics_20.png)| The [Simple Arithmetics](Examples/Arithmetics/SimpleArithmetics) project shows how to perform simple computations with some basic console input/output. |
|![Sinus1](Images/Sinus1_20.png)| The [Sinus1](Examples/Arithmetics/Sinus1) project outputs a simple sinus graf in console mode. |
|![Sinus2](Images/Sinus2_20.png)| The [Sinus2](Examples/Arithmetics/Sinus2) project outputs a simple sinus graf in raster graphics mode. |

### Text Screen Manipulation

The [Text Screen Manipulation](Examples/Text Screen Manipulation) category contains a list of projects showing how you can manipulate the text 
screen directly and modify character sets to create interesting applications.

| Screen Shot | Project description |
|-------------|---------------------|
|![Bouncing Character 1](Images/BouncingCharacter1_20.png)| The [Bouncing Character 1](Examples/Text Screen Manipulation/BouncingCharacter1) project shows how you can use direct screen manipulation to make a character bounce around the screen. |
|![Bouncing Character 2](Images/BouncingCharacter2_20.png)| The [Bouncing Character 2](Examples/Text Screen Manipulation/BouncingCharacter2) project adds objects on the screen to the [Bouncing Character 1](Examples/Text Screen Manipulation/BouncingCharacter1) project with which the character can interact by bouncing against them. |
|![Bouncing Character 3](Images/BouncingCharacter3_20.png)| The [Bouncing Character 3](Examples/Text Screen Manipulation/BouncingCharacter3) project adds simple user interaction though the keyboard to the [Bouncing Character 2](Examples/Text Screen Manipulation/BouncingCharacter2) project. |
|![Bouncing Character 4](Images/BouncingCharacter4_20.png)| The [Bouncing Character 4](Examples/Text Screen Manipulation/BouncingCharacter4) project customizes the characters in [Bouncing Character 3](Examples/Text Screen Manipulation/BouncingCharacter3) project and shows how this technique can be used to create more interesting character-based user interfaces. |
|![Bouncing Character 5](Images/BouncingCharacter5_20.png)| The [Bouncing Character 5](Examples/Text Screen Manipulation/BouncingCharacter5) project adds sound to the [Bouncing Character 4](Examples/Text Screen Manipulation/BouncingCharacter4) project, and plays a sound effect when the character bounces. |
|![Create Labyrinth](Images/CreateLabyrinth_20.png)| The [Create Labyrinth](Examples/Text Screen Manipulation/CreateLabyrinth) project creates a random labyrinth on the screen and lets a small entity randomly walk around in the labyrinth. |

### Raster Graphics

Applications introducing raster graphics are available in the [Raster Graphics](Examples/Raster Graphics) category. The applications show how
to perform different simple graphics operations.

### Sprites

Sprites are available in all screen modes, and provide a mechanism to display movable objects, possibly animated, on top of the screen. The
projects in the [Sprites](Examples/Sprites) category display different uses for sprites.

### Games

Finally, the [Games](Examples/Games) category contain more complete applications using the retro-environment to create a retro-game.