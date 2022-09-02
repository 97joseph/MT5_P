# MT5_P
 Assests Predictor
 
 97joseph/MT5_P

(( Ai-INPUTS ))
1. Price Data
— All Timeframes
— Open/High/Low/Close
2. Average Spread Monitor
— Uses Ai to find average spread
— For “MaxSpread” in the EA
3. Correlation
— All Timeframes
— Uses Ai to find price-move relationships between all symbols data in watch-list.
4. Average True Range
— All Timeframes
— Updates every new candlestick
— Uses Ai to calculate the “ATR” from the “Open” of each candlestick. Plots a line, same width as candlestick, Above&Below (Entry/StopLoss/TakeProfit)


(( Entry Conditions ))
— New ATR strangle on each candlestick
— BUY: (ABOVE-ATR)(PendingOrder)
1. Once price touches, SELL trade cancels
— SELL: (BELOW-ATR)(PendingOrder)
1. Once price touches, BUY trade cancels
— Ai confirms each entry via correlation (Ai-Confidence%)

=====

(( AutoTrader Settings ))
1. Ai-Confidence%:
2. MaxSpread: (Average Spread Monitor)
3. Risk%: (Equity)
4. ATR-StopLoss: Static//Trailing
5. ATR-TakeProfit: Static//Trailing
6. MaxOpenTrades:
7. MaxDailyProfit(%): (Equity)
8. MaxDailyDrawDown(%): (Equity)
