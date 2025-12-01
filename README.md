# Frequency-Model-Caddie-Reaserch
Frequency grid based on monthly volatility for trading intraday assets.

This repository contains a technical indicator developed in NTSL (Nelogica Trading System Language) for the ProfitChart platform.

The tool's objective is to project a volatility trading grid based on market frequencies (HFT/Legs) from a reference point.

Features

Dynamic Adjustment Base: The algorithm automatically captures the closing price of the 4 PM candle from the previous day to use as a base (Official Adjustment Proxy). If there is no data, it uses the closing price of the previous day (CloseD(1)).

Extensive Grid (31 Levels): Projects 15 resistance levels and 15 support levels, totaling 31 reference lines on the chart.

Real Plotting: Uses native plotting commands (Plot up to Plot31) to draw physical lines, allowing for better visualization and individual color configuration.

Parameterization: The frequency (range size) is fully configurable via input.

How to Install

Open ProfitChart.

Access the Strategies menu > Strategy Editor.

Click New and paste the code from the .prt file in this repository.

Save it as GridFrequenciaTotal.

Compile the code.

The indicator assumes that the market moves at standard frequencies (deviations or legs of HFT).

Yellow Line: Reference Price (Adjustment/16h).

Green Lines: Resistance Levels (+1 freq, +2 freq...).

Red Lines: Support Levels (-1 freq, -2 freq...).

Developed for institutional and professional trader use.
