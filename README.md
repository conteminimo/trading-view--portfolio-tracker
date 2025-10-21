# trading-view--portfolio-tracker
This Pine Script indicator plots your average cost basis on any stock chart and displays the real-time percentage gain or loss.

Portfolio Tracker for TradingView
This indicator provides a simple yet powerful way to visualize your portfolio holdings directly on your TradingView charts. It plots a horizontal line at your average cost for any stock in your portfolio and displays a clean, dynamic label showing the percentage difference between your cost basis and the current price.

This tool is perfect for investors who want an at-a-glance view of their positions without needing to switch between their broker and their charting platform.

How It Works
The script contains a simple if/else if block where you can hard-code your portfolio positions. For each stock, you define its unique Ticker ID (including the exchange prefix, e.g., "BATS:AMZN") and your average cost.

When you view a chart, the script checks if the current ticker matches one in your list. If a match is found, it automatically draws the horizontal line at your average cost and activates the percentage label. For any chart not in your list, the indicator remains hidden.

Features
Custom Portfolio: Easily add your entire portfolio with specific average cost prices for each holding.

Visual Cost Basis: A clear, solid green line is plotted on the chart at your average cost for a quick visual reference.

Dynamic Percentage Label: A clean label, attached to the current price, shows the real-time percentage gain or loss from your average cost.

Clean UI: The line and label only appear on charts for stocks that are in your portfolio, keeping other charts uncluttered.

How to Use
Add the indicator to your chart.

Open the Pine Editor and find the section marked // --- ⚙️ YOUR PORTFOLIO SETTINGS ---.

Modify the if/else if list with your personal portfolio data, adding or removing stocks as needed. Ensure the Ticker ID is an exact match for what TradingView uses for that symbol.

Save the script. The indicator will now automatically display your data on the relevant charts.

How to Sync with TradingView
Since there is no direct Git integration, the workflow is manual:

Make all edits to your script in your local .pine file.

Commit your changes using Git to keep a clean history.

Copy the entire code from your local file.

Paste it into the TradingView Pine Editor and save.
