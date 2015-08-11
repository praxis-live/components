# Custom Components

SubGraph (.pxg) files are a way of reusing and sharing custom components or groups of components for use with [Praxis LIVE](http://www.praxislive.org)

## Usage

Download the [latest zip file](https://github.com/praxis-live/pxg/archive/master.zip) and extract the contents. Drag .pxg files into your patch from the File Browser tab, or import them into your palette (choose `Import` from the popup menu on palette categories).

## Components

Under active development - lots more to come!

### Core

Components that can be used in any graph (audio, video, tinkerforge, etc.).

* `seconds.pxg` - Output running time in seconds.

### Video

Components that can be used in any video graph.

* `colourbalance.pxg` - alter the rgb balance of a video input.
* `xform.pxg` - 2D transform (translate, scale, rotate) a video input.

### VideoGL

Video components that can only be used with the OpenGL renderer.

* `fx-kaleidoscope.pxg` - kaleidoscope effect with controllable number of segments. GLSL code derived from https://github.com/neilmendoza/ofxPostProcessing/blob/master/src/KaleidoscopePass.cpp
* `fx-pinch.pxg` - pinch image effect.
* `gl-filter-base.pxg` - GLSL filter base - add to graph and edit fragment (GLSL) and code (Java).
* `xform-3d.pxg` - translate and rotate a video input in 3D space.

## Create your own SubGraph (.pxg) file

There is not currently a way to export SubGraph files, however they are easy to create. Simply select the component(s) you wish to reuse within the patcher window. Open your favourite text editor, and copy & paste the selected components from Praxis LIVE into the editor. Save the resulting text file with a .pxg extension. You can then drag this file from the File Manager into the patcher window.

Please share!
