# IT Rsi EA

This is the code for the IT RSI EA, developed by Forex Robot Easy Team. For detailed reviews and trading results of this product, visit [this link](https://forexroboteasy.com/forex-robot-review/it-rsi-ea-review-optimize-forex-trades-with-mt4s-rsi-strategy/).

## Description

IT Rsi EA is an expert advisor that utilizes the RSI (Relative Strength Index) strategy to optimize forex trades. It opens sell trades when the RSI value is above the overbought level and opens buy trades when the RSI value is below the oversold level. The EA allows customization of input parameters such as RSI period, overbought level, oversold level, lot size, stop loss, and take profit.

Please note that Forex Robot Easy is not the official developer of this product. We only provide a sample code that can work as described in this product. To find the official developer of this product, please refer to MQL5.

## Input Parameters

- **rsiPeriod**: RSI period (default: 14)
- **overboughtLevel**: Overbought level (default: 70)
- **oversoldLevel**: Oversold level (default: 30)
- **lotSize**: Lot size (default: 0.01)
- **stopLoss**: Stop loss in pips (default: 100)
- **takeProfit**: Take profit in pips (default: 200)

## Initialization Function

The `OnInit()` function is called during expert initialization. Any necessary initialization code can be added here.

## Deinitialization Function

The `OnDeinit()` function is called when the expert is being deinitialized. Any necessary deinitialization code can be added here.

## Tick Function

The `OnTick()` function is called on every tick of the chart. It retrieves the RSI value and checks for overbought and oversold conditions. If the conditions are met, it opens sell or buy trades accordingly.

## Sell Trade Function

The `SellTrade()` function is called to open a sell trade. It calculates the stop loss and take profit levels based on the current Ask price and the input parameters. It then sends an order to sell with the specified lot size, stop loss, and take profit.

## Buy Trade Function

The `BuyTrade()` function is called to open a buy trade. It calculates the stop loss and take profit levels based on the current Bid price and the input parameters. It then sends an order to buy with the specified lot size, stop loss, and take profit.
