# Coding isn't Programming

[Closing Keynote with Leslie Lamport](https://www.socallinuxexpo.org/scale/22x/presentations/closing-keynote-leslie-lamport)

Leslie Lamport

Microsoft Research Emeritus

## Regarding Abstractions
- Things about concurrent programs apply to all programs
- Algorithms are higher level than programs
- Distributed programs are just convenient programs with threads on different machines
- Find the correct algorithm for the concurrent part (the small but important part)
- Use abstractions
- Programmers need to think at higher level than code to code well

### Need to know
1. *What* the program does
2. *How* to do it 

## TLA+ Program Modeling
- TLA+ to describe abstractions of concurrent algorithms
- Can you find a *what* that makes the code simpler (bargaining on requirements)

_(algorithm example with empty sets and what is the smallest number)_

- Next step of computer programs can only depend on current state, not previous (but current state can encapsulate past state) 
- TLA+ at AWS: Formal methods to check correctness
- European Space Agency Virtuoso project used TLA+
- Related book: Formal Development of a Network-Centric RTOS Software Engineering for Reliable Embedded Systems
- TLA TeX: pretty printer for TLA+
- Easier to debug the abstraction than the rules
- Need to write in order to think: "If you're thinking, but not writing, you only think that you're thinking"
- Don't get hung up on languages, especially programming languages

## Bonus (over time) slides
- Why programs should have bugs
- Programs can only have bugs if there is a precise description of what a program does
- W3C used definitions of inputs/outputs to define correctness

## Questions
- AI validation is hard
- Bridging open source with modern academia? Microsoft Research always saw improving the science through publishing as a goal
- Dealing with frustration of not seeing algorithms well defined before programming? Agile appears to be popular because programmers don't like talking to customers. Think more.
