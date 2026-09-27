# C++ Limit Order Book & Matching Engine

> 🚧 **WORK IN PROGRESS — This project is actively being developed.**

A C++ implementation of a simplified exchange-style limit order book and matching engine.

The engine is intended to explore:

* C++ data structures
* Order matching
* Price-time priority
* Memory management
* Algorithmic complexity
* Performance measurement
* Latency and throughput
* Systems-level optimization

## Current Status

**Early development.**

The order representation, order-book data structures, matching logic, cancellation system, testing strategy, and performance architecture are still being developed.

Nothing in this README should be considered final.

## Planned Architecture

```text
Incoming Orders
       │
       ▼
┌─────────────────┐
│ Matching Engine │
└────────┬────────┘
         │
         ▼
┌─────────────────────────┐
│      Order Book         │
│                         │
│   Bids       Asks       │
│    │          │         │
│    ▼          ▼         │
│ Price Levels / Queues   │
└──────────┬──────────────┘
           │
           ▼
      Trade Events
```

## Planned Features

### Core

* Limit orders
* Bid/ask books
* Price-time priority
* Matching
* Partial fills
* Multiple fills

### Order Management

* Order IDs
* Cancellation
* Order states
* Market orders

### Testing & Benchmarking

* Automated correctness tests
* Throughput measurements
* Latency measurements
* p50 / p95 / p99 latency
* Memory measurements

### Performance Investigation

* Data-structure comparisons
* Memory allocation
* Cache locality
* Object lifetime
* Memory pools / custom allocation strategies

## Engineering Philosophy

The project will prioritize:

```text
CORRECTNESS
     ↓
MEASUREMENT
     ↓
PROFILE
     ↓
OPTIMIZE
     ↓
BENCHMARK AGAIN
```

Performance claims will only be made after being measured.

Concurrency and more advanced exchange functionality will be considered only after the single-threaded implementation is correct and understood.

## Development Status

Current milestone:

**Project setup and order-book design.**

More documentation will be added as the project develops.
