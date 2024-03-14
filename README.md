# Paula Bollinger Bands Strategy

This code is an implementation of the Paula Bollinger Bands strategy, developed by Joe Ross. The strategy uses Bollinger Bands to identify potential trade entry points.

## Indicator Initialization

In the `OnInit()` function, the Bollinger Bands indicator is created and configured. The indicator is named 'Paula Bollinger Bands' and its style is set to draw a line. The indicator buffer is set to `ExtMapBuffer` and labeled as 'Bollinger Bands'.

## Indicator Calculation

In the `OnCalculate()` function, the Bollinger Bands are calculated for each bar in the chart. The calculation starts from the first uncalculated bar and continues until the last bar.

The Bollinger Bands are calculated using the Bollinger Bands formula, which involves calculating the moving average (MA) and standard deviation. The upper band is calculated as the MA plus a multiple of the standard deviation, and the lower band is calculated as the MA minus the same multiple of the standard deviation.

The indicator buffer is filled with the closing prices of each bar.

The code also checks for trade entry conditions. If the previous bar's closing price is above the upper band and the current bar's closing price is below the upper band, a potential trade entry is identified. The subsequent bar's closing price is then checked to ensure it falls within the bands. If all conditions are met, the `ExecuteTrade()` function is called to execute the trade.

## Execute Trade

The `ExecuteTrade()` function is a placeholder function that should be implemented with the actual trade execution logic. This function is called when a trade entry condition is met.

## Product Description

The Paula Bollinger Bands strategy is a trading strategy developed by Joe Ross. It utilizes the Bollinger Bands indicator to identify potential trade entry points. The strategy is implemented in the code provided.

To use this strategy, simply apply the indicator to your chart and wait for trade entry signals. The strategy looks for situations where the previous bar's closing price is above the upper band and the current bar's closing price is below the upper band. It then checks if the subsequent bar's closing price falls within the bands. If all conditions are met, a trade is executed.

Please note that this code is provided as a sample and is not the official implementation of the Paula Bollinger Bands strategy. ForexRobotEasy is not the official developer of this product. For detailed reviews and trading results of the official product, please visit the following link: [Paula Bollinger Bands Review](https://forexroboteasy.com/forex-robot-review/paula-bollinger-bands-review-of-joe-rosss-forex-strategy/).

For the official developer of this product and to access the complete implementation, please use MQL5.
