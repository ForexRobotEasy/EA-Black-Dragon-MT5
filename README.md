# EA Black Dragon MT5

[![Forex Robot Easy](https://forexroboteasy.com/wp-content/uploads/2019/07/ForexRobotEasyLogo.png)](https://forexroboteasy.com/forex-robot-review/ea-black-dragon-mt5-review-indicator-based-forex-software/)

## Overview
EA Black Dragon MT5 is an indicator-based Forex trading robot developed by the Forex Robot Easy Team. This code serves as a sample implementation of the EA Black Dragon MT5 trading strategy.

For detailed reviews and trading results of the official product, please visit the [Forex Robot Easy website](https://forexroboteasy.com/forex-robot-review/ea-black-dragon-mt5-review-indicator-based-forex-software/).

## Prerequisites
Before running this code, ensure that the following libraries and indicators are included:

- PositionInfo.mqh
- Trade.mqh
- BlackDragon.mqh
- MovingAverages.mqh

## Configuration
The code includes several global variables that can be customized based on individual trading strategies and preferences:

- `enableHedging`: Set to `true` to enable trading on accounts that support hedging.
- `enableNewSeries`: Set to `true` to enable opening a new series of orders.
- `stopLossMultiplier`: Defines the multiplier for modifying the stop loss level.
- `networkMultiplier`: Defines the multiplier for modifying the network of orders.
- `fastMA`: Defines the period for the fast moving average.
- `slowMA`: Defines the period for the slow moving average.

## Functions
### `OpenDealBasedOnIndicatorColor()`
This function opens a new deal based on the color of the Black Dragon indicator. If the color is green, a buy order is placed. If the color is red, a sell order is placed.

### `ManageOrdersBasedOnIndicatorColor()`
This function manages the existing orders based on the color of the Black Dragon indicator. If the color is green, the stop loss level and network of orders are modified. If the color is red, only the stop loss level is modified.

### `EnableHedging()`
This function enables trading on accounts that support hedging, if the `enableHedging` variable is set to `true`.

### `CustomizeSettings()`
This function can be used to add custom settings specific to individual trading strategies and preferences.

### `EnableOrDisableNewSeries()`
This function enables or disables the opening of a new series of orders, based on the value of the `enableNewSeries` variable.

### `ManageMovingAverages()`
This function manages the moving averages by retrieving the values of the fast and slow moving averages using the `GetMAValue()` method from the `CMovingAverages` object. Custom moving averages management logic can be added in this function.

### `TradeOperations()`
This function executes the trading operations by calling the above-defined functions in the required sequence.

### `OnStart()`
This is the entry point of the program. It calls the `TradeOperations()` function to start the trading process.

## Disclaimer
Please note that ForexRobotEasy is not the official developer of this product. The provided code is a sample implementation that can work as described in the official product. To find the official developer of this product and for detailed reviews and trading results, please visit the [Forex Robot Easy website](https://forexroboteasy.com/forex-robot-review/ea-black-dragon-mt5-review-indicator-based-forex-software/).
