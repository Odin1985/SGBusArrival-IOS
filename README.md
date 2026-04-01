# SGBusArrival-IOS

A native iOS & watchOS app for real-time Singapore bus arrival times, built with SwiftUI and WidgetKit.

## Features

- **Real-time Bus Arrivals** — Live ETAs from LTA DataMall API for any bus stop in Singapore
- **Nearest Stop Detection** — Automatically finds the closest bus stop using GPS
- **Load Indicators** — See bus occupancy at a glance (Seats Available, Standing, Limited Standing)
- **Bus Type Info** — Single Deck (SD) / Double Deck (DD) identification
- **Favourites** — Save frequently used bus stops for quick access

## Widgets

### iPhone Home Screen
| Size | Description |
|------|-------------|
| **Small** (2x2) | Top 3 buses with next ETA |
| **Medium** (4x2) | 3 buses with load indicators + 3 arrival columns (Next/2nd/3rd) |
| **Large** (4x4) | Full bus list with load, type, and 3 ETAs per service |

### iPhone Lock Screen
| Type | Description |
|------|-------------|
| **Circular** | Single bus ETA in a compact circle |
| **Rectangular** | Two buses with ETAs side by side |
| **Inline** | Compact strip above the clock |

### Apple Watch Complications
| Type | Description |
|------|-------------|
| **Circular** | Single bus service ETA |
| **Circular Gauge** | ETA with countdown ring visual |
| **Rectangular** | Two buses + stop name |
| **Modular Large** | 3 buses with load indicators (center complication) |
| **Extra Large** | 4 buses with primary + secondary ETAs |
| **Smart Stack** | watchOS 10+ scrollable widget card |

### Apple Watch App
- Full bus arrival list with load indicators
- NavigationStack-based UI
- Crown scrollable bus stop list

## Design Preview

Open `docs/widget-designs.html` in a browser to view all widget mockups rendered as interactive iOS-native styled previews, including iPhone mockups and Apple Watch face previews.

## Tech Stack

- **SwiftUI** — Declarative UI framework
- **WidgetKit** — Home screen, lock screen & watch widgets
- **ClockKit** — Apple Watch complications
- **CoreLocation** — Nearest bus stop detection
- **LTA DataMall API** — Singapore real-time bus arrival data

## API

This app uses the [LTA DataMall](https://datamall.lta.gov.sg/) API for real-time bus arrival data. You will need an API key from LTA to run the app.

## Requirements

- iOS 17.0+
- watchOS 10.0+
- Xcode 15.0+

## License

MIT License
