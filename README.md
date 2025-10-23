# HyperOrderbook Visualization

A simple, standalone HTML visualization tool for HyperLiquid orderbook data. No server required - just open in your browser!

## Features

- Interactive orderbook depth chart
- Real-time price and volume metrics
- Detailed tooltips on hover
- File upload support for orderbook data
- Clean, modern interface

## Usage

1. Open `index.html` in your web browser
2. Click the file input button
3. Select your orderbook data file (JSON/TXT format)
4. View the interactive visualization

## Data Format

The tool expects orderbook data in the following JSON format:
```json
{
  "time": "...",
  "raw": {
    "channel": "l2Book",
    "data": {
      "coin": "...",
      "time": 1234567890,
      "levels": [
        [{"px": "0.1234", "sz": "100.0", "n": 1}],  // bids
        [{"px": "0.1235", "sz": "100.0", "n": 1}]   // asks
      ]
    }
  }
}
```

## Features

- Bid/Ask visualization
- Cumulative depth chart
- Price levels
- Order sizes
- Number of orders per level
- Total volumes
- Best bid/ask prices
- Market spread

## Tech Stack

- D3.js for visualization
- Pure HTML/CSS/JavaScript
- No dependencies
- No server required

## License

GPL-3.0 license
