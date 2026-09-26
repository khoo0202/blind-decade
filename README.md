# Blind Decade

A browser game that teaches the basics of investing using real U.S. market history, with the years hidden.

You start with $10,000 and save $300 every month. Each month you read the news, buy or sell, and then end the month. Your rival is the "lazy investor", who puts every dollar into an S&P 500 fund and never sells. When the decade is over, the game reveals which real period you just lived through.

**Play:** https://khoo0202.github.io/blind-decade/

## What's in the game

- **Instant trades, manual time.** Trades fill immediately. Time only moves when you press "End month".
- **7 funds / ETFs:** S&P 500, U.S. Treasuries, gold, 3x leveraged S&P 500, tech, high dividend, emerging markets.
- **6 random stocks per game,** drawn from 16 fictional companies. Each one secretly turns out to be a superstar, a steady blue chip, an ordinary company, a slow decliner, a blow-up (sometimes delisted), or a turnaround.
- **Life events and decisions:** year-end bonuses, raises, surprise bills that can force you to sell, a friend's "hot tip", panic in a bear market, and the temptation of leverage in a bull market.
- **20 knowledge cards** that pop up when your actions trigger them (compounding, inflation, drawdowns, panic selling, chasing gains, concentration risk, fees, emergency funds...), 6 of them with a short quiz.
- **Modes:** a random 10-year decade, a quick 5 years, and 5 historical levels (1929, 1972, 1997, 2005, 2016).
- **End-of-game report** with an S–D grade, your key decisions, and 12 achievements. Cards and achievements are saved in your browser.

The game interface is in Chinese.

## Data

- S&P 500: Robert Shiller's monthly data (from 1928, dividends included, monthly average prices), via [datasets/s-and-p-500](https://github.com/datasets/s-and-p-500).
- Gold: monthly prices from [datasets/gold-prices](https://github.com/datasets/gold-prices).
- Treasuries are estimated from the 10-year yield; cash earns roughly the 10-year yield minus 1.2%; the 3x fund is 3 times the real monthly S&P 500 move (real products lose more to daily rebalancing).
- The tech, high-dividend and emerging-market ETFs and all individual stocks are simulated, linked to the real market, and randomized every game.
- Dividends, rates and inflation after late 2023 are extended from the last known values.

Everything runs in a single `index.html` file with no build step and no external requests except Google Fonts.

This is a learning game, not financial advice.
