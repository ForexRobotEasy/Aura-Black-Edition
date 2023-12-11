# Aura Black Edition

This is the code for the Aura Black Edition Forex robot developed by the Forex Robot Easy Team. For detailed reviews and trading results of this product, please visit [here](https://forexroboteasy.com/forex-robot-review/aura-black-edition-review-stable-gold-trading-ea/).

## Developer Information

- Developer: Forex Robot Easy Team
- Developer's Site: [forexroboteasy.com](https://forexroboteasy.com)

## Introduction

The Aura Black Edition is an automated trading robot designed to trade the XAUUSD (Gold) symbol. It uses a feedforward neural network to analyze market conditions and make trading decisions. This code provides the necessary functions to manage risk, execute trades, and monitor the trading account.

## Code Structure

The code is structured into several functions:

1. `TradeGold()` - This function checks the market conditions, calculates stop loss and take profit levels, opens a position, adjusts the trading strategy based on market conditions, and closes the oldest position if the maximum number of positions is reached.

2. `ManageRisk()` - This function calculates the position size based on the account balance and desired risk, and sets the leverage control.

3. `ExecuteTrades()` - This function gets trade signals from the neural network, executes trade entry if there is a valid entry signal, and closes all open positions if there is an exit signal.

4. `MonitorAccount()` - This function gets the account balance and equity, and outputs the account information.

5. `OnTick()` - This is the main function that is called on each tick. It manages risk, executes trades, and monitors the account.

## Usage

To use the Aura Black Edition Forex robot, you need to include the required classes (`Trade` and `FeedforwardNeuralNetwork`) and define the necessary constants (`SYMBOL`, `LOT_SIZE`, `MAX_POSITIONS`).

The main function `OnTick()` is called on each tick and manages the overall trading process. It calls the other functions to manage risk, execute trades, and monitor the account.

## Note

Please note that ForexRobotEasy is not the official developer of this product. This code is provided as a sample that demonstrates how the product described in the link above may work. To find the official developer of this product, please use MQL5.
