# DayNightSystem

This is a very simple System, its ease to integrate into existing projects and extend if needed.

[Marktplace Url](https://www.unrealengine.com/marketplace/en-US/product/226f49f1b9c24c44830986dad86869ed)

## Included Assets

#### BP_DefaultGameMode

Base game mode, used to configure custom blueprint classes. Use as example for your custom game mode.

#### BP_DefaultGameState

Store the current time, and serve it for all clients playing on server.

#### BP_DefaultPlayerController

Store the user specific clock type preference, and draw the widgets on player viewport.

#### BP_WeatherManager

This is where the magic happens. When placed in the level you can configure the custom settings and set a reference for the world directional light, also BP_DefaultGameState must be set in your game mode. (**This is extremely important, if this is not done the system will not work properly**).

Some of the custom settings:

| Setting                    | Description                                               | Default    |
| -------------------------- | --------------------------------------------------------- | ---------- |
| DayCycleSpeed              | Sets the speed that time passes                           | 1          |
| StartDate                  | Defines the date that the system will start counting      | 00/00/0000 |
| EnableCalendar             | If should count months and years or only days             | true       |
| DaysPerMonth               | How many days in a month                                  | 30         |
| MonthPerYear               | How many months in a year                                 | 12         |
| TemperatureFlutuationCurve | Custom temperature variation curve                        | CurveAsset |
| BaseWorldTemperature       | The base world temperature                                | 20         |
| BasTemperatureMultiplier   | The value to multiply for the base world temperature      | 1          |
| WorldTemperatureVariation  | How mutch the temperature must variate, for more and less | 10         |

*If you set 1 to DayCycleSpeed, 1 in game day will be 1 hour in real world*

New options come in future releases.

#### FL_Temperature

Store usefull functions for work with diferent temperature metrics.

#### WB_Preview

Simple widget blueprint for format and display the current temperature, date and time.

#### Example Map

Base map showing the system working.

#### Custom Enums and Structs

Used for store some values and create new variable types.

## Author

Guilherme Werner
