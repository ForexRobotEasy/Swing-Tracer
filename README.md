# Swing Tracer ReadMe

This is the ReadMe file for the Swing Tracer software developed by the Forex Robot Easy Team. 

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Swing Tracer Review](https://forexroboteasy.com/forex-robot-review/swing-tracer-review-enhance-forex-trading-with-atr-based-software/). Please note that ForexRobotEasy is not the official developer of this product. We are only providing a sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

## Overview

The Swing Tracer is an indicator designed for MetaTrader 5 platform. It helps to identify swing highs and swing lows in the price chart based on the Average True Range (ATR) indicator. Swing highs are marked with an upward arrow, while swing lows are marked with a downward arrow.

## Features

- Customizable ATR period
- Customizable colors for swing highs and swing lows
- Maximum number of notifications can be set
- Sends notifications when the maximum number of swing points is reached

## Installation

1. Copy the 'Swing Tracer.mq5' file into the 'Indicators' folder of your MetaTrader 5 installation directory.
2. Restart MetaTrader 5 or refresh the indicators list.
3. Open the chart you want to apply the indicator to.
4. Drag and drop the 'Swing Tracer' indicator onto the chart.

## Inputs

- **ATRPeriod** (default: 14): The period used for calculating the Average True Range (ATR).
- **DefaultColor** (default: Blue): The color of the swing points that are not part of a trend.
- **TrendColor** (default: Red): The color of the swing points that are part of a trend.
- **MaxNotifications** (default: 5): The maximum number of swing points to be marked before sending a notification.

## Indicator Buffers

- **buffer1**: Contains the swing highs. The indicator draws an upward arrow at these points.
- **buffer2**: Contains the swing lows. The indicator draws a downward arrow at these points.

## Initialization Function

The `OnInit()` function is called during the indicator initialization process. In this function, the indicator buffers are set, along with their respective styles and labels. The indicator properties such as short name and description are also set.

## Iteration Function

The `OnCalculate()` function is called for each new tick of data. In this function, the ATR is calculated using the `iATR()` function. Then, the indicator checks for swing highs and swing lows based on the conditions specified. If a swing high or swing low is detected, the corresponding buffer is updated and the notifications count is incremented. If the maximum number of swing points is reached, a notification is sent and the notifications count is reset.

## Contact Information

For any inquiries or support regarding this product, please visit [Forex Robot Easy](https://forexroboteasy.com) website.

---

Please note that this ReadMe file is for informational purposes only and should not be considered as financial advice. Trading in the Forex market carries significant risks and it is important to carefully consider your investment objectives, level of experience, and risk appetite before participating in the market.
