# OSS Mega Jam

## Overview

The OSS Mega Jam is a collaborative open-source game development initiative focused on:
- shipping small polished games
- learning through collaboration
- building reusable tooling
- encouraging intentional human creativity
- maintaining healthy contributor culture
- releasing public playable games every development cycle

Each Mega Jam cycle lasts approximately 3 months and concludes with a public release on platforms such as Steam or itch.io.

---

## OSS Mega Jam Discord Server
### [Join the community here](https://discord.gg/paGhdzckd5)



---



# Core Philosophy

## Build Small, Ship Often

The project prioritizes:
- finished experiences
- maintainable systems
- contributor accessibility
- scoped gameplay ideas

Over:
- endless feature expansion
- premature engine development
- overengineering
- abandoned prototypes

---

# Technology Stack

## Framework

The current official framework is:

- MonoGame
- C#
- GitHub for version control and collaboration

## Why MonoGame?

MonoGame was selected because it:
- reduces onboarding friction
- improves contributor accessibility
- avoids manual memory management concerns
- allows faster iteration
- provides strong tooling support
- keeps development focused on game creation rather than engine complexity

---

# Repository Structure

Example structure:
 
```text
/assets
/audio
/content
/docs
/shaders
/src
    /core
    /game
    /systems
/tools

```


### This is an example of bad documentation
```c#

   
    // This prints the number x amount of time.
    public void PrintNumbers(int amount){
        
        // This is the loop for printing numbers.
        for (int i = 0; i <= amount; i++){
            
            // This is what writes to the console.
            Console.WriteLine("The value is {i}"); // This isn't printing right, we need to fix it.
        }
    }
    
```
   ### This is an example of good documentation 
```c#
 
   
    /// <summary>
    /// This prints the selected amount of number the user wants.
    /// </summary>
    /// <param name="amount">This is how many times you want it to print starting from 0</param>
    public void PrintNumbers(int amount){
        for (int i = 0; i <= amount; i++){
            Console.WriteLine("The value is {i}"); // TODO: Fix the output "The value is {i}"
        }
    }
    
    
```

### What is the difference?
The major difference between them is the amount of information. You do not need to tell us what each line does. The code should be self-explanatory. When in doubt, follow [Monogame's Source Code](https://github.com/MonoGame/MonoGame/blob/develop/MonoGame.Framework/Color.cs).

Please do not stress about being perfect. This is a project meant to learn and have fun. You will not, and are not expected to do everything perfectly. Just have a good time and let's make a game.


# AI Policy
While we at OSS Mega Jam aren't against the use of AI for coding, we will be barring use of it for any and all OSS Mega Jam projects. The only permitable usage of AI will be only for tab-complete. But not copy and paste bult amount.

While we understand that AI is growing at an exorbinate rate, we do feel that for your own growth and understanding of what you are working on, we can't in best concious allowed for AI code, art, music, and expertise. Any use of it outside of tab-completion will be immediately denied on the merge.
