# Editor Guide

This guide is up to date as of v1.5.343

<details>
  <summary>Here's what's not yet added to the guide</summary>

	- Everything is currently up to date
</details>

## Table of contents

- [Editor Guide](#editor-guide)
	- [Table of contents](#table-of-contents)
	- [Introduction](#introduction)
		- [Controls](#controls)
	- [Interface](#interface)
		- [Sidebar](#sidebar)
		- [Sidebar: Helper features](#sidebar-helper-features)
		- [Sidebar: Editor modes](#sidebar-editor-modes)
		- [Editor Modes: Build](#editor-modes-build)
		- [Editor Modes: Edit](#editor-modes-edit)
		- [Editor Modes: Delete](#editor-modes-delete)
		- [Editor Modes: Paint](#editor-modes-paint)
	- [Your First Level](#your-first-level)
		- [Building the layout](#building-the-layout)
		- [Start and Checkpoints](#start-and-checkpoints)
		- [Testing](#testing)
		- [Decorating](#decorating)
		- [Validating and Sharing](#validating-and-sharing)
	- [Advanced editing](#advanced-editing)
		- [Road Node](#road-node)
		- [Road options](#road-options)
		- [Pipe Node Options](#pipe-node-options)
		- [Pipe Properties](#pipe-properties)
		- [Portals](#portals)
		- [Start Line](#start-line)
		- [Checkpoints](#checkpoints)
		- [LED Boards](#led-boards)
		- [Prism Shape](#prism-shape)
		- [Lights](#lights)

## Introduction

The editor allows you to create your own levels, which can later be shared online with other players.

All the different features might be daunting at first, but this guide will help you get started, and will hopefully enable you to create some great levels!

### Controls

**Note**: The editor currently only supports keyboard and mouse controls. Controller support is _not_ planned for the foreseeable future.

Freefly camera:
| `R-Click` (hold) | Look Around |
|-|-|
| `W` `A` `S` `D` | Move Camera |
| `LShift` (hold) | Move Faster

General:
| `L-Click` | Place/Select |
|-|-|
| `Scroll Up/Down` | Move Grid Up/Down |
| `PageUp`/`PageDown` | Move Grid Up/Down |
| `Shift` + `Scroll` | Rotate current object (Yaw) |
| `Ctrl` + `Scroll` | Rotate current object (Roll) |
| `Alt` + `Scroll` | Rotate current object (Pitch) |
| `R` | Reset object rotation |

Miscellaneous:
| `Ctrl` + `Z` | Undo |
|-|-|
| `Ctrl` + `Y` | Redo |
| `Ctrl` + `S` | Save |

## Interface

When entering the editor, you will be greeted with the following interface:

![alt text]({4AC4CCF3-D75D-40FF-8F4E-831BF1B54E2C}.png)

Let's go over the different parts of the interface!

### Sidebar

The editor sidebar is where you can access the main functionalities of the editor

![alt text](image-1.png)

### Sidebar: Helper features

The editor comes with some helpful features to streamline track creation:

![alt text](image-2.png)

Here is what all of them do:

1. **X-Ray:** will show a faint _ghost_ of objects behind other objects. This is useful if for not getting lost with your item placements
  ![alt text](ezgif-442e80cba0573de6.gif)
2. **Fullbright:** makes the map visible in the dark. This is useful for nigh-time maps. _Note:_ this is **_editor only_**. Driving the map will return brightness back to normal
  ![alt text](fullbright.gif)
3. **Reset Camera:** this will teleport you back to the middle of the map. Useful when you end up _"going into the stratosphere"_
  ![alt text](reset_cam.gif)
4. **Undo/Redo:** Pretty self explanatory. This is for those who either _can't make up their mind_ or just keep _messing up_ :eyes:
	- Note: you can also use `Ctrl` + `Z`/`Y`
  ![alt text](undo_redo.gif)
5. **Metadata:** This is where you can set the _metadata_ for your track. This includes _Track Name_ and _Number of Laps_
  ![alt text](metadata.gif)
6. **Save:** _I don't need to explain this..._

### Sidebar: Editor modes

These modes are the main way you can create your track. 

![alt text](image-3.png)

1. **Build:** _place new items_
2. **Edit:** _modify existing items_ (position, color, etc.)
3. **Delete:** _remove existing items_
4. **Scenery:** _modify the landscape_ (time/weather, paint mountains, etc.)
5. **Paint (WIP):** _mass modify existing items_ (currently only allows to edit surface type on roads)
6. **Test:** allows to drive the track (details later)

### Editor Modes: Build

In this mode, you can _place new items_ on the map. 

![alt text](image-4.png)

1. **Road:** Flat surfaces for driving with a multitude of parameters (surface, support beams, runoff, fences, etc.)
2. **Pipe:** Circular tubes for driving
3. **Portal:** Portal gates where which can teleport the car
4. **Start:** Place the start line or edit its size
5. **Checkpoints (CP):** used for keeping track of the player's progress on track and as respawn points
6. **LED Board:** Large Decorative boards, with option to use custom textures
7. **Prism:** Polygon Prism shapes for decoration, with option to use custom textures
8. **Light:** Circular- and Spotlights for lighting up your track

### Editor Modes: Edit

Clicking on an item in `Edit` mode lets you move it, rotate it and change its properties (for more info on properties see [Advanced editing](#advanced-editing))

![a](editing.gif)


### Editor Modes: Delete

Clicking on an item in `Delete` mode will delete that item

![a](deleting.gif)

### Editor Modes: Paint

Clicking on an item in `Paint` mode will let you change its surface type. This currently only works on roads and pipes

![a](painting.gif)


## Your First Level

Now that you know how to navigate around the editor, let's create your first track!

First, let's start the editor with a fresh, empty canvas:

> ![alt text](image-6.png)
> 
> Go to `Build` Menu and press `New`

### Building the layout

> ![alt text](image-7.png)
>
> **Tip:** You can close property menus for now, so you have more ✨_screen estate_✨ 

You will first be presented with a little _yellow arrow_, this is used for placing down _road pieces_ by connecting them.

Simply place down these arrows by clicking where you wanna place them.

![a](place_roads.gif)

You can change the height by _Scrolling with the mouse_

Additionally, you can rotate the arrow (or any placeable element), using:
- `Shift` + `Scroll` to rotate its direction
- `Ctrl` + `Scroll` to make it tilted
- `Alt` + `Scroll` to rotate its elevation up and down
  
**Tip:** Clicking on an existing _arrow_ will automatically connect your road to it

You can also place down tube shaped roads, by going to the `Pipe` submenu on the left

![alt text](image-8.png)

These essentially work the same, as placing flat roads, but they use a _blue_ arrow

![a](place_pipes.gif)

> ![alt text](image-9.png)
>
> **Note:** you should place these higher on the grid, because the arrow marks the _middle_ of the tube shape, which may lead to you placing the tube underground

Once you created a general layout of your track, you should place the a _Start Line_, to mark the starting point of the track

### Start and Checkpoints

**Important:** Every track must contain a _Start Line_ and _at least one Checkpoint_ for it to be valid!

> ![alt text](image-10.png)
>
> Go to the `Start` submenu


Now you can place the _Start Line_ to where you want your track to start

![a](place_start.gif)

Be mindful of the arrow's direction, as that marks which way your car will face!

---

To make your track functional, you also have to palce _Checkpoints_. These will keep track of the player's progress throughout the track, and can also serve as _respawn points_ in case someone goes off-track

**Note:** during a race, a lap will only count if the player went through all the Checkpoints. Place these in critical parts of the track, to keep players from taking unwanted shortcuts

> ![alt text](image-11.png)
>
> Go to the `Checkpoint` submenu

Place down a couple _Checkpoints_ around your track's layout.

![alt text](place_cp.gif)

Be mindful so the _little white dot_ is **above** the ground (that marks roughly where the car will respawn); also make sure that the the arrow is facing the right direction.

With this, you have built a very basic track.

### Testing

You can test how the track feels while driving using the _test mode_

> ![alt text](image-13.png)
>
> Go to the `Test` submenu

A preview of the car will appear at your mouse cursor. Clicking anywhere will place the car there, and you can test driving around.

![a](test_mode.gif)

**Tip:** You can also directly click on the _Start Line_ or on a _Checkpoint_, and it will place the car at the corresponding element's spawn position. This is useful to verify respawn points and that the _Start Line_ is placed correctly.

**Tip:** you can respawn during _Testing_, just like in-game. 
- Press `Enter` to respawn to the last _Checkpoint_ you crossed 
- Press `Backspace` to respawn to the initial location where you started testing
- Press `Esc` to cancel testing and go back to editing


### Decorating

To spice up the track, you can place down different decorations. Let's start with the _LED Boards_

> ![alt text](image-14.png)
>
> Go to the `Build` -> `LED Board` submenu


![alt text](image-15.png)

You will have different option to choose from. The most interesting one is the _Texture_

> ![alt text](image-16.png)
>
> Multitude of pre-existing textures for different situations

Select the texture you like, and place down youe _LED board_

![a](place_led_board.gif)

Not finding anything related to what you want to place? You can also use custom textures!

![alt text](image-17.png)

1. Toggle on the `Use Custom Texture` option
2. Paste a URL to your image of liking
3. Press `Enter` to apply it
4. You can now place down an _LED Board_ with any custom texture
> ![a](custom_led_texture.gif)
> 
> [Image Used](https://preview.redd.it/remeber-who-you-are-v0-knpemw9pm92h1.png?auto=webp&s=10ff63da22b929b7d6d6508211af7ac84f472fd2)

---

You can also make the surrounding landscape more interesting with the _Scenery Editor_

> ![alt text](image-19.png)
>
> Go to the `Scenery` submenu

1. **Landscape editing tools:** allows you to create mountains/valleys and shape the ladscape
2. **Time of day/Weather:** allows you to change the time of day and adjust the weather

![a](landscape_editing.gif)

Using the `Normal` brush, and _Raise/Lower_, you can raise or lower the height of the landscape as you please.

Using the `Flatten` brush, you can create areas of flat ground. Wherever you started painting, that height becomes the _target height_, and painting over areas will raise/lower those to this height, resulting in a flat ground


You can set the mood of your track using the time and weather sliders.

![a](time_weather.gif)

Using the `Time of Day` slider, you can create daytime/nighttime tracks

Using the `Cloudiness` slider, you can change how many clouds are visible

Using the `Gloominess` slider, you can change the type of clouds, from happy ☀️ to sad 🌧️

### Validating and Sharing

Once you're happy with your track, you can give it a name and set the number of laps.

> ![alt text](image-20.png)
>
> Open the `Metadata` screen

1. Give your track a name
2. Set the desired number of laps
3. **_Make sure_** to save any changes

> ![alt text](image-21.png)
>
> The editor will notify you whenever your track is saved

Now that the track is done, you can share it online so other players can play it. To do this, you first have to validate it.

> ![alt text](image-22.png)
>
> Exit the editor, select your track and press `Validate`

You will now be required to finish your track and set a time, which will be used to calculate the medals for the track (Bronze, Silver, Gold)

![a](validate.gif)

You can choose to improve your time, to make achieving medals on your track more challenging. The game will choose the best time you performed as the medal time when uploading your track.

Once you're happy with your time, you can upload it to the servers

> ![alt text](image-23.png)
>
> 1. Select your track
> 2. Press upload
> 3. A confirmation window will pop-up if the upload was successful

![alt text](image-24.png)

Your track is now available for play to all players!

## Advanced editing

For more professional looking tracks, the editor comes with advanced features as well.

**Note:** there are a lot of features with differing complexitites. Take your time to familiarize yourself with them and feel free to come back to _this guide_ whenever your feeling lost

You can see these option either when placing down your items, or by going to the `Edit` mode and selecting an item you want to edit

### Road Node

Properties that you can change in the `Road Node Options` menu apply to only _one end_ of your road piece.

![alt text](image-25.png)

1. **Road Profile:** different profile for your road. It can have an indent, a bump, or just be chaotic
2. **Profile Height:** how large the currently set `Profile` height is
3. **Width:** how wide the road is
4. **Left/Right Runoff:** useful for adding runoff areas. The players can cut the track here, with a penalty to their speed

![a](road_node_properties.gif)

### Road options

You can change properties of the road you drive on in the `Road Options` menu, such as surface type, support beams or walls

![alt text](image-26.png)

1. **Surface Material:** the surface type, with different driving properties
2. **Wall Material:** what the walls are made of
3. **Support Type:** useful to _ground_ the track, so it is not just floating in the sky
4. **Support Material:** what the supports are made of
5. **Support Bottom:** useful if the supports don't quite reach the ground
6. **Wall Type:** what the shape walls are
7. **Wall Start Height:** what height the walls starts at
8. **Wall End Height:** what height the walls ends at
9. **Runoff Material:** what the runoff surface is made of

![a](road_properties.gif)

### Pipe Node Options

Properties that you can change in the `Pipe Node Options` menu apply to only _one end_ of your pipe piece.

![alt text](image-27.png)

1. **Radius:** how wide the tube is
2. **Profile:** how open or closed the tube is; using `360°` will created a fully closed tube
3. **Flat:** if the tube is circular or flat; useful for connecting the tube to flat road pieces

![a](pipe_node_properties.gif)

### Pipe Properties

You can change the surface type of the tube here

![a](pipe_properties.gif)

### Portals

Placing down portals one after another will automaticaly link them. You can also manually set links later if you decide so

![alt text](image-28.png)

1. **Portal ID:** the ID of the currently selected poral. Useful for linking
2. **Linked ID:** the ID of the currently linked portal
3. **Unlink:** pressing this will destroy the link. The portal will lead nowhere
4. **Change Link:** useful for manually linking portals
5. **Width/Height:** change the size of the portal
6. **Color options:** 
   - **Portal Color:** the color of the portal swirl. Will also change what color it glows in
   - **Frame Color:** the color of the metal frame around the portal
   - **Rust Color:** the color of the rust on the metal frame
   - **Rust Intensity:** how rusty the frame is. Setting it to `0.0` will result in a _clean, pristine_ frame
7. **Bottom Frame:** toggle if the portal is open at the bottom or not. Should be turned _ON_ in case the portal is placed in the air, or `OFF` of the portal is on the ground
	- **Important note:** going from an open portal to a closed one might cause the car to snag on the bottom frame and get bumped

> ![a](portal_properties.gif)
>
> Showcasing the editable properties
> 
> Changing the `Width`/`Height` parameters will change the linked portal's size as well

> ![a](portal_linking.gif)
>
> How to unlink portals and create a link manually
>
> Note down the portal's ID you want to link, enter it to the other portal's `Change Link` field, then press `Link`


### Start Line

You can change the size of the _Start Line_

**Note:** you can only have one _Start Line_ on the map. Trying to place a new one will delete the old one

![a](start_line.gif)

### Checkpoints

You can change the size and thickness of _Checkpoints_

![a](checkpoints.gif)

### LED Boards

![alt text](image-29.png)

1. **Width/Height:** change the size of the board
2. **Support Beams:** whether or not the board has support structure; useful if you want to attach a board to an existing structure
3. **Support Bottom:** how low the support structure goes; useful when you place boards higher in the air, the structure doesn't quite reach the ground
4. **Use Custom Texture:** whether or not the board uses a custom texture. See [Decorating](#decorating) on how to use this
5. **Texture:** which texture to display on the board

![a](led_board.gif)

### Prism Shape

Prism shapes allow you to place prism or pyramid like shapes, such as cubes, elongated hexagons, pyramids with any number of sides, etc.

![alt text](image-30.png)

1. **Surface Type:** how the surface act when driving on it
2. **Width/Height/Depth:** the dimensions of the shape
3. **Sides:** how many sides the shape has
4. **Pointy:** toggling this on will turn the shape into a pyramid
5. **Sharp:** Whether the shape will look smooth or jagged (useful when trying to create poles or pillars shapes, with sides 12+)
6. **Texture options:** you can set what texture is used on the top, sides and bottom. Allow custom textures, just like [LED Boards](#decorating)

![a](prism_shape.gif)

### Lights

![alt text](image-31.png)

1. **Color:** the color of the light
2. **Spotlight:** whether the light is circular (like a lightbulb), or directional (like a headlight)
3. **Size:** essentially how bright the light is

![a](lights_demo.gif)


> ![a](light_circles.gif)
> 
> Note: the spheres where you place the lights are only visible **_while editing_**.


