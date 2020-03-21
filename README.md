# visum

## Workflow setup

### Binaries

- hie (mouse hover) (not available for latest ghc version, need previous stack resolver)
- ormolu (CTRL+Shift+I)

### Vscode Extensions

- Haskell syntax Highlighting
- Haskell Language Server
- ormolu

### Libs

- sdl2
- reactive-banana
- reactive-banana-sdl2

### hie.yaml

"cradle: stack: component: "visum:lib""

## Vision

This library is a combination of a lot of different conceptual and implementation ideas and will likely change dramatically over time.
Ultimately, I just want a library where *achieving* a task is only as complex as concieving of the solution.
There's a difference between the specifying of user interfaces being time-consuming and it being so complex, error-prone and unpredictable that you can't get work done
The HTML,CSS,JS,DOM,... stack is exactly this. Various libraries attempt to contol the chaos that these things spew and give you a peaceful layer of abstraction to work upon. But they can only do so much. And when this abstraction eventally leaks, you lose all faith in humanity and/or your ability to get your project done in the way you wanted.

Some ideas I think are important:

- Continuous space (vector graphics)
- Continuous movement (vector animation)
- Continuous time (FRP)
- Clean abstraction layers
- Low level: akin to declarative svg creation, but with facility to specify signals/channels/events and also animations
- High level: akin to dragging and dropping google's material components
- Declarative and pure semantics from the bottom up
- Widget = GUI App. We compose Larger Apps out of smaller ones.
- Primitives for building 2D visuals based on SVG and Wikipedia suggestions
- Animations = Linear transformations
- Rational co-ordinate system?
