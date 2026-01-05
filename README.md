# 2026 Senate Forecast

Interactive visualization of the 2026 US Senate election forecast.

**[View the forecast →](https://evand.github.io/2026-senate-forecast/)**

## Features

- **Hex map** of Senate races color-coded by probability (blue = D likely, red = R likely)
- **Snake chart** showing races sorted by competitiveness (tipping point analysis)
- **Conditional filtering** - lock outcomes to see "what-if" scenarios
- **Correlation analysis** - see which races move together
- **Statistical uncertainty** - ESS and confidence intervals displayed

## Methodology

Probabilities are derived from [Manifold Markets](https://manifold.markets/) prediction markets using maximum entropy sampling with market constraints. The model:

1. Takes individual race markets as marginal probability constraints
2. Takes aggregate markets (Senate control, etc.) as joint constraints
3. Samples from the maximum entropy distribution consistent with all constraints
4. Identifies where markets are inconsistent (statistical arbitrage opportunities)

## Data

- **35 races**: 33 Class II seats + 2 special elections (OH, FL)
- **Baseline**: 31 R, 34 D-caucus (32 D + 2 I) not up for election
- **Control threshold**: Democrats need 51 seats (17 wins from 35 races)

Last updated: January 2026

## License

MIT - Data from Manifold Markets under their terms of service.
