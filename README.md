# DayNightSystem

This is a very simple System, its ease to integrate into existing projects and extende if needed.

[Marktplace Url](https://www.unrealengine.com/marketplace/en-US/product/226f49f1b9c24c44830986dad86869ed)

## Included Assets

#### BP_DefaultGameMode

Base game mode, used to configure custom blueprint classes. Use as example for your custom game mode.

#### BP_DefaultGameState

Store the current time, and serve it for all clients playing on server.

#### BP_DefaultPlayerController

Store the user specific clock type preference, and draw the widgets on player viewport.

#### BP_TimeManager

This is where the magic happens. When placed in the level you can configure the custom settings and set a reference for the world directional light. (**This is extremely important, if this is not done the system will not work properly**).

Some of the custom settings:

| Setting               | Description                                              | Default  |
| --------------------- | -------------------------------------------------------- | -------- |
| DayCycleSpeed         | Sets the speed that time passes                          | 1        |
| StartTime             | Defines the date that the system will start counting     | 0        |

*If you set 1 to DayCycleSpeed, 1 in game day will be 1 hour in real world*

New options come in future releases.

#### WB_Clock

Simple widget blueprint for format and display the current date and time.

#### Example Map

Base map showing the system working.

#### Custom Enums and Structs

Used for store some values and create new variable types.

## Author

Guilherme Werner
