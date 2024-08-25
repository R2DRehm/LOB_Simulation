# LOB Simulation - Simplified Markovian Order Book

This repository simulates a limit order book (LOB) using a simplified Markovian model. It generates dynamic order flows, processes events, and visualizes the bid-ask spread evolution. Below is an overview and analysis of the core functionality and implementation details.

## Overview

The project uses Python libraries like NumPy, Pandas, and Matplotlib for simulation and visualization. It handles different types of orders (market, limit, cancel) and simulates their effects on the order book over time.

### Core Components

- **`Queue` class**: Represents the bid or ask side of the order book.
- **`Carnet` class**: Manages the order book and updates its state after every event.
- **`Ordre` class**: Encapsulates an order with a type (market, limit, cancel) and direction (buy, sell).

### Libraries Used

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from numpy.random import default_rng
from matplotlib.animation import FuncAnimation
