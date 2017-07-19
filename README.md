# fdf
A quirky wireframe software renderer

## Motivation

fdf is the introductory graphics project in the [42](https://en.wikipedia.org/wiki/42_(school)) curriculum.

The basic requirement is to load a file who's format is as follows:
```
0 0 10 10 0
0 0 10 10 0
````
That makes a wireframe and the number is the elevation where the wire's intersect.
This fdf also supports rudimentary wavefront obj files, rendered as quads.
There are a variety of controls to make rendering more interesting.
But why quirky? Well, triangles do not have colors smoothly interpolated
across their face. Rather, you have a blend of colors mimicking, a poorly calibrated
thermal camera, based on the orientation of the object.

## Compatability

Tested on Mac 10.9.5 - 10.10.5

## Getting started

```
$> make
$> ./fdf ./example.fdf
````

## Keyboard Commands

### Transformation

#### Rotation

<kbd>&rightarrow;</kbd> - +x

<kbd>&uparrow;</kbd> - +y

<kbd>&leftarrow;</kbd> +z

#### Translation

<kbd>T</kbd> - +X

<kbd>G</kbd> - -X

<kbd>Y</kbd> - +Y

<kbd>H</kbd> - -Y

<kbd>U</kbd> - +Z (The camera is looking down the positive Z axis)

<kbd>J</kbd> - -Z

#### Scale

<kbd>Q</kbd> - +X

<kbd>A</kbd> - -X

<kbd>W</kbd> - +Y

<kbd>S</kbd> - -Y

<kbd>E</kbd> - +Z

<kbd>D</kbd> - -Z

### Colors

Let it rip on the <kbd>1</kbd> through <kbd>9</kbd> to shift the colors.

