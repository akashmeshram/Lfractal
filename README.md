# Lfractal
(This is new react implementation, older raw version is available [here](https://github.com/akashmeshram/Lfractal-html-version))
<p align="center"><img src="https://user-images.githubusercontent.com/30370067/116772719-7cb08600-aa6e-11eb-8311-6c77236feb0e.jpg"></p>

##  Table of Contents
- [About](#about)
- [Demo](#demo)
- [Usage](#usage)
- [Author](#authors)
- [References](#references)
- [License](#license)

## About <a name = "about"></a>
An  L-system is a parallel string rewriting system. A string rewriting system consists of an initial string, called the seed, and a set of rules for specifying how the symbols in a string are rewritten as (replaced by) strings. 

The recursive nature of the L-system rules leads to self-similarity and thereby fractal-like forms which are easy to describe with an L-system. Plant models and natural-looking organic forms 'grow' and becomes more complex by increasing the iteration level of the form.

<!-- ## Demo <a name = "demo"></a> -->
<!-- <p align="center"><img src="./lsystem.gif"></p> -->

## Usage <a name = "usage"></a>
Following character have geometric interpretation.

|Character  |      Meaning|
| ------------- |:-------------:| 
|   F	      |     Move forward by line length drawing a line|
|   f	      |     Move forward by line length without drawing a line|
|   +	      |     Turn left by turning angle|
|   -	      |     Turn right by turning angle|
|   \|	      |     Reverse direction (ie: turn by 180 degrees)|
|   \[       |      Push current drawing state onto stack|
|   \]	      |     Pop current drawing state from the stack|
  
Change the following parameters to get different systems

|Parameters| Meaning|
| ------------- |:-------------:| 
| `AXIOM`  | initial string |
| `RULES`  | rewriting rule|
| `STARTX` | canvas starting width position|
| `STARTY` | canvas starting height position|
| `LENGTH` | step size|
| `ANGLE`  | degree of direction change|

Then increase (or decrease) `ITERATIONS` to get next iteration


## Author <a name = "authors"></a>
- [Akash Meshram](https://github.com/akashmeshram) 

## References <a name = "references"></a>
- Grzegorz Rozenberg and Arto Salomaa. The mathematical theory of L systems (Academic Press, New York, 1980).
- Przemysław Prusinkiewicz, Aristid Lindenmayer – The Algorithmic Beauty of Plants.
- Kari, Lila; Rozenberg, Grzegorz; Salomaa, Arto (1997). "L Systems".

## License <a name = "license"></a>
Copyright © 2021 [Akash Meshram](https://github.com/akashmeshram).<br />
This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details
