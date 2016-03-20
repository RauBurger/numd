# Numd
A numerical methods library for the [D Programming language](https://dlang.org).

## Intro
Numd is my attempt at a numerical methods library written in the [D Programming language](https://dlang.org).
So far it contains a number of optimization algorithms (that desperately need to be refactored), a handful of differentiation
methods, one integrator and a currently evolving linear algebra package.

I started this project for a class I took during my undergrad. The class itself was
focused on optimization methods, which I implemented in D, but as I went I was displeased
with D's mathematics and numerical method library support (sorry scid). I wanted a more 
~~object oriented~~ TEMPLATES!! (or whatever I feel appropriate) approach so I decided to write my own, based off what I had done for class.

## Things planned at this point:
- More differentiation (2nd order, 3rd order, cental, left, right, ...)
- ODE solvers (Euler, ~~RK~~(done-ish), Adams, ...)
- PDE solvers (Lax-Friedrichs, Lax-Wendoff, Upwind, ...)
- Interpolators (some of these will support various ODE and PDE methods)
- Linear algebra (from basic matrix ops to more advanced things, eigensystems and whatnot)
- Check out [RPP](https://github.com/Rob-Rau/rpp) ~~Plotting (current lame implementation is based off plplot, want to roll my own)~~

## TODO:
- ~~Make it easy to build and use.~~
	- ~~Fix absolute path dependencies~~
	- ~~Set up Cmake or some other build system~~
	- I'm using dub now
- Write some unit regression tests
	- This is in preparation for TODO 5
- Write basic matrix library
	- Basic matrix object and ops (addition, multiplication, inverse)
- Clean up optimization library to use the new matrix library
	- Replace blas matrix function with new shiny objects.
- Start implementing the above list in no particular order.
	- With the rest in place this shouldn't be to hard....lol

## Dependencies:
- cblas
- scid
