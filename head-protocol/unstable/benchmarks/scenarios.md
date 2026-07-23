--- 
sidebar_label: 'Scenario benchmarks' 
sidebar_position: 5 
--- 

# Scenario benchmark results 

This page collects results from the scenario matrix: every combination  of cluster size, UTxO shape, and incremental-ops mode is exercised by  CI from the latest `master` code and reported below.

:::caution

Numbers are approximate. They come from cloud VMs rather than  controlled hardware, so the useful signal is the relative change  between cells and between commits, not the absolute throughput.

:::

_Generated at_  2026-07-23 07:08:34.122818352 UTC


## Summary across cells

TPS columns are rates (transactions per second); _Wall clock (s)_ is the measured elapsed time from the first tx submission to the last confirmation. Times are rounded to one decimal.

| Scenario | Txs | Wall clock (s) | End-to-end TPS (tx/s) | Sustained TPS (tx/s) | Avg conf (ms) | P95 conf (ms) |
| -- | -- | -- | -- | -- | -- | -- |
| Nodes=1, Constant, incremental ops off, fire and forget | 30 | 0.1 | 572.51 | n/a | 51.6 | 52.1 |
| Nodes=1, Constant, incremental ops off, wait for tx valid | 30 | 0.2 | 180.68 | 178.95 | 5.5 | 7.2 |
| Nodes=1, Growing, incremental ops off, fire and forget | 30 | 0.1 | 437.77 | n/a | 67.4 | 68.3 |
| Nodes=1, Growing, incremental ops off, wait for tx valid | 30 | 0.2 | 120.24 | 118.42 | 8.3 | 11.7 |
| Nodes=1, Mixed, incremental ops off, fire and forget | 30 | 0.1 | 533.89 | n/a | 55.2 | 55.9 |
| Nodes=1, Mixed, incremental ops off, wait for tx valid | 30 | 0.2 | 141.99 | 138.03 | 7.0 | 8.8 |
| Nodes=2, Constant, incremental ops off, fire and forget | 60 | 0.1 | 420.15 | n/a | 140.6 | 142.5 |
| Nodes=2, Constant, incremental ops off, wait for tx valid | 60 | 0.5 | 118.87 | 119.78 | 16.7 | 20.7 |
| Nodes=2, Growing, incremental ops off, fire and forget | 60 | 0.2 | 377.93 | n/a | 156.1 | 158.4 |
| Nodes=2, Growing, incremental ops off, wait for tx valid | 60 | 0.9 | 70.21 | 69.73 | 28.2 | 38.8 |
| Nodes=2, Mixed, incremental ops off, fire and forget | 60 | 0.1 | 432.59 | n/a | 137.0 | 138.4 |
| Nodes=2, Mixed, incremental ops off, wait for tx valid | 60 | 0.7 | 86.20 | 82.08 | 23.0 | 34.0 |
| Nodes=3, Constant, incremental ops off, fire and forget | 90 | 0.2 | 368.68 | n/a | 239.3 | 242.5 |
| Nodes=3, Constant, incremental ops off, wait for tx valid | 90 | 0.9 | 99.84 | 99.83 | 29.4 | 39.9 |
| Nodes=3, Growing, incremental ops off, fire and forget | 90 | 0.3 | 298.89 | n/a | 297.5 | 300.2 |
| Nodes=3, Growing, incremental ops off, wait for tx valid | 90 | 1.7 | 52.75 | 53.92 | 54.7 | 83.8 |
| Nodes=3, Mixed, incremental ops off, fire and forget | 90 | 0.3 | 328.91 | n/a | 270.6 | 272.5 |
| Nodes=3, Mixed, incremental ops off, wait for tx valid | 90 | 1.2 | 72.71 | 67.81 | 41.0 | 55.9 |


## Nodes=1, Constant, incremental ops off, fire and forget



| Number of nodes |  1 | 
| -- | -- |
| _Number of txs_ | 30 |
| _Avg. Confirmation Time (ms)_ | 51.6 |
| _P99_ | 52.1ms |
| _P95_ | 52.1ms |
| _P50_ | 51.8ms |
| _Tx validation time p50 (ms)_ | 22.0 |
| _End-to-end TPS_ | 572.51 tx/s |
| _Backlog drain time (s)_ | 0.1 |
| _Snapshots observed_ | 2 |
| _Snapshots per second_ | 38.17 /s |
| _Avg txs per snapshot_ | 15.0 |
| _Peak node RSS (MB)_ | 154.9 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 2 |
      

## Nodes=1, Constant, incremental ops off, wait for tx valid



| Number of nodes |  1 | 
| -- | -- |
| _Number of txs_ | 30 |
| _Avg. Confirmation Time (ms)_ | 5.5 |
| _P99_ | 7.8ms |
| _P95_ | 7.2ms |
| _P50_ | 5.2ms |
| _Tx validation time p50 (ms)_ | 1.8 |
| _End-to-end TPS_ | 180.68 tx/s |
| _Sustained TPS_ | 178.95 tx/s |
| _Backlog drain time (s)_ | 0.0 |
| _Snapshots observed_ | 30 |
| _Snapshots per second_ | 180.68 /s |
| _Avg txs per snapshot_ | 1.0 |
| _Peak node RSS (MB)_ | 155.6 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 2 |
      

## Nodes=1, Growing, incremental ops off, fire and forget



| Number of nodes |  1 | 
| -- | -- |
| _Number of txs_ | 30 |
| _Avg. Confirmation Time (ms)_ | 67.4 |
| _P99_ | 68.3ms |
| _P95_ | 68.3ms |
| _P50_ | 67.8ms |
| _Tx validation time p50 (ms)_ | 26.6 |
| _End-to-end TPS_ | 437.77 tx/s |
| _Backlog drain time (s)_ | 0.1 |
| _Snapshots observed_ | 2 |
| _Snapshots per second_ | 29.18 /s |
| _Avg txs per snapshot_ | 15.0 |
| _Peak node RSS (MB)_ | 152.7 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 31 |
      

## Nodes=1, Growing, incremental ops off, wait for tx valid



| Number of nodes |  1 | 
| -- | -- |
| _Number of txs_ | 30 |
| _Avg. Confirmation Time (ms)_ | 8.3 |
| _P99_ | 15.7ms |
| _P95_ | 11.7ms |
| _P50_ | 7.9ms |
| _Tx validation time p50 (ms)_ | 1.8 |
| _End-to-end TPS_ | 120.24 tx/s |
| _Sustained TPS_ | 118.42 tx/s |
| _Backlog drain time (s)_ | 0.0 |
| _Snapshots observed_ | 30 |
| _Snapshots per second_ | 120.24 /s |
| _Avg txs per snapshot_ | 1.0 |
| _Peak node RSS (MB)_ | 159.9 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 31 |
      

## Nodes=1, Mixed, incremental ops off, fire and forget

Each client first grows its UTxO set (1-in to 2-out) for half of its tx budget, then contracts it back (2-in to 1-out) for the remainder.

| Number of nodes |  1 | 
| -- | -- |
| _Number of txs_ | 30 |
| _Avg. Confirmation Time (ms)_ | 55.2 |
| _P99_ | 55.9ms |
| _P95_ | 55.9ms |
| _P50_ | 55.4ms |
| _Tx validation time p50 (ms)_ | 23.0 |
| _End-to-end TPS_ | 533.89 tx/s |
| _Backlog drain time (s)_ | 0.1 |
| _Snapshots observed_ | 2 |
| _Snapshots per second_ | 35.59 /s |
| _Avg txs per snapshot_ | 15.0 |
| _Peak node RSS (MB)_ | 158.6 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 2 |
      

## Nodes=1, Mixed, incremental ops off, wait for tx valid

Each client first grows its UTxO set (1-in to 2-out) for half of its tx budget, then contracts it back (2-in to 1-out) for the remainder.

| Number of nodes |  1 | 
| -- | -- |
| _Number of txs_ | 30 |
| _Avg. Confirmation Time (ms)_ | 7.0 |
| _P99_ | 14.4ms |
| _P95_ | 8.8ms |
| _P50_ | 6.5ms |
| _Tx validation time p50 (ms)_ | 1.8 |
| _End-to-end TPS_ | 141.99 tx/s |
| _Sustained TPS_ | 138.03 tx/s |
| _Backlog drain time (s)_ | 0.0 |
| _Snapshots observed_ | 30 |
| _Snapshots per second_ | 141.99 /s |
| _Avg txs per snapshot_ | 1.0 |
| _Peak node RSS (MB)_ | 158.9 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 2 |
      

## Nodes=2, Constant, incremental ops off, fire and forget



| Number of nodes |  2 | 
| -- | -- |
| _Number of txs_ | 60 |
| _Avg. Confirmation Time (ms)_ | 140.6 |
| _P99_ | 142.6ms |
| _P95_ | 142.5ms |
| _P50_ | 140.7ms |
| _Tx validation time p50 (ms)_ | 53.3 |
| _End-to-end TPS_ | 420.15 tx/s |
| _Backlog drain time (s)_ | 0.1 |
| _Snapshots observed_ | 2 |
| _Snapshots per second_ | 14.00 /s |
| _Avg txs per snapshot_ | 30.0 |
| _Peak node RSS (MB)_ | 152.6 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 3 |
      

## Nodes=2, Constant, incremental ops off, wait for tx valid



| Number of nodes |  2 | 
| -- | -- |
| _Number of txs_ | 60 |
| _Avg. Confirmation Time (ms)_ | 16.7 |
| _P99_ | 23.0ms |
| _P95_ | 20.7ms |
| _P50_ | 16.1ms |
| _Tx validation time p50 (ms)_ | 5.7 |
| _End-to-end TPS_ | 118.87 tx/s |
| _Sustained TPS_ | 119.78 tx/s |
| _Backlog drain time (s)_ | 0.0 |
| _Snapshots observed_ | 60 |
| _Snapshots per second_ | 118.87 /s |
| _Avg txs per snapshot_ | 1.0 |
| _Peak node RSS (MB)_ | 154.1 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 3 |
      

## Nodes=2, Growing, incremental ops off, fire and forget



| Number of nodes |  2 | 
| -- | -- |
| _Number of txs_ | 60 |
| _Avg. Confirmation Time (ms)_ | 156.1 |
| _P99_ | 158.5ms |
| _P95_ | 158.4ms |
| _P50_ | 156.2ms |
| _Tx validation time p50 (ms)_ | 57.2 |
| _End-to-end TPS_ | 377.93 tx/s |
| _Backlog drain time (s)_ | 0.2 |
| _Snapshots observed_ | 2 |
| _Snapshots per second_ | 12.60 /s |
| _Avg txs per snapshot_ | 30.0 |
| _Peak node RSS (MB)_ | 153.1 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 62 |
      

## Nodes=2, Growing, incremental ops off, wait for tx valid



| Number of nodes |  2 | 
| -- | -- |
| _Number of txs_ | 60 |
| _Avg. Confirmation Time (ms)_ | 28.2 |
| _P99_ | 45.7ms |
| _P95_ | 38.8ms |
| _P50_ | 28.4ms |
| _Tx validation time p50 (ms)_ | 9.2 |
| _End-to-end TPS_ | 70.21 tx/s |
| _Sustained TPS_ | 69.73 tx/s |
| _Backlog drain time (s)_ | 0.0 |
| _Snapshots observed_ | 60 |
| _Snapshots per second_ | 70.21 /s |
| _Avg txs per snapshot_ | 1.0 |
| _Peak node RSS (MB)_ | 156.7 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 62 |
      

## Nodes=2, Mixed, incremental ops off, fire and forget

Each client first grows its UTxO set (1-in to 2-out) for half of its tx budget, then contracts it back (2-in to 1-out) for the remainder.

| Number of nodes |  2 | 
| -- | -- |
| _Number of txs_ | 60 |
| _Avg. Confirmation Time (ms)_ | 137.0 |
| _P99_ | 138.5ms |
| _P95_ | 138.4ms |
| _P50_ | 136.9ms |
| _Tx validation time p50 (ms)_ | 58.8 |
| _End-to-end TPS_ | 432.59 tx/s |
| _Backlog drain time (s)_ | 0.1 |
| _Snapshots observed_ | 2 |
| _Snapshots per second_ | 14.42 /s |
| _Avg txs per snapshot_ | 30.0 |
| _Peak node RSS (MB)_ | 152.7 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 3 |
      

## Nodes=2, Mixed, incremental ops off, wait for tx valid

Each client first grows its UTxO set (1-in to 2-out) for half of its tx budget, then contracts it back (2-in to 1-out) for the remainder.

| Number of nodes |  2 | 
| -- | -- |
| _Number of txs_ | 60 |
| _Avg. Confirmation Time (ms)_ | 23.0 |
| _P99_ | 35.9ms |
| _P95_ | 34.0ms |
| _P50_ | 22.5ms |
| _Tx validation time p50 (ms)_ | 6.2 |
| _End-to-end TPS_ | 86.20 tx/s |
| _Sustained TPS_ | 82.08 tx/s |
| _Backlog drain time (s)_ | 0.0 |
| _Snapshots observed_ | 60 |
| _Snapshots per second_ | 86.20 /s |
| _Avg txs per snapshot_ | 1.0 |
| _Peak node RSS (MB)_ | 156.1 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 3 |
      

## Nodes=3, Constant, incremental ops off, fire and forget



| Number of nodes |  3 | 
| -- | -- |
| _Number of txs_ | 90 |
| _Avg. Confirmation Time (ms)_ | 239.3 |
| _P99_ | 242.7ms |
| _P95_ | 242.5ms |
| _P50_ | 238.5ms |
| _Tx validation time p50 (ms)_ | 103.8 |
| _End-to-end TPS_ | 368.68 tx/s |
| _Backlog drain time (s)_ | 0.2 |
| _Snapshots observed_ | 2 |
| _Snapshots per second_ | 8.19 /s |
| _Avg txs per snapshot_ | 45.0 |
| _Peak node RSS (MB)_ | 152.7 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 4 |
      

## Nodes=3, Constant, incremental ops off, wait for tx valid



| Number of nodes |  3 | 
| -- | -- |
| _Number of txs_ | 90 |
| _Avg. Confirmation Time (ms)_ | 29.4 |
| _P99_ | 43.5ms |
| _P95_ | 39.9ms |
| _P50_ | 28.2ms |
| _Tx validation time p50 (ms)_ | 7.3 |
| _End-to-end TPS_ | 99.84 tx/s |
| _Sustained TPS_ | 99.83 tx/s |
| _Backlog drain time (s)_ | 0.0 |
| _Snapshots observed_ | 61 |
| _Snapshots per second_ | 67.67 /s |
| _Avg txs per snapshot_ | 1.5 |
| _Peak node RSS (MB)_ | 153.9 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 4 |
      

## Nodes=3, Growing, incremental ops off, fire and forget



| Number of nodes |  3 | 
| -- | -- |
| _Number of txs_ | 90 |
| _Avg. Confirmation Time (ms)_ | 297.5 |
| _P99_ | 300.3ms |
| _P95_ | 300.2ms |
| _P50_ | 299.5ms |
| _Tx validation time p50 (ms)_ | 104.1 |
| _End-to-end TPS_ | 298.89 tx/s |
| _Backlog drain time (s)_ | 0.3 |
| _Snapshots observed_ | 2 |
| _Snapshots per second_ | 6.64 /s |
| _Avg txs per snapshot_ | 45.0 |
| _Peak node RSS (MB)_ | 153.4 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 0 |
      

## Nodes=3, Growing, incremental ops off, wait for tx valid



| Number of nodes |  3 | 
| -- | -- |
| _Number of txs_ | 90 |
| _Avg. Confirmation Time (ms)_ | 54.7 |
| _P99_ | 100.4ms |
| _P95_ | 83.8ms |
| _P50_ | 53.9ms |
| _Tx validation time p50 (ms)_ | 16.4 |
| _End-to-end TPS_ | 52.75 tx/s |
| _Sustained TPS_ | 53.92 tx/s |
| _Backlog drain time (s)_ | 0.0 |
| _Snapshots observed_ | 62 |
| _Snapshots per second_ | 36.34 /s |
| _Avg txs per snapshot_ | 1.5 |
| _Peak node RSS (MB)_ | 157.6 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 0 |
      

## Nodes=3, Mixed, incremental ops off, fire and forget

Each client first grows its UTxO set (1-in to 2-out) for half of its tx budget, then contracts it back (2-in to 1-out) for the remainder.

| Number of nodes |  3 | 
| -- | -- |
| _Number of txs_ | 90 |
| _Avg. Confirmation Time (ms)_ | 270.6 |
| _P99_ | 272.6ms |
| _P95_ | 272.5ms |
| _P50_ | 271.7ms |
| _Tx validation time p50 (ms)_ | 111.7 |
| _End-to-end TPS_ | 328.91 tx/s |
| _Backlog drain time (s)_ | 0.3 |
| _Snapshots observed_ | 2 |
| _Snapshots per second_ | 7.31 /s |
| _Avg txs per snapshot_ | 45.0 |
| _Peak node RSS (MB)_ | 153.9 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 4 |
      

## Nodes=3, Mixed, incremental ops off, wait for tx valid

Each client first grows its UTxO set (1-in to 2-out) for half of its tx budget, then contracts it back (2-in to 1-out) for the remainder.

| Number of nodes |  3 | 
| -- | -- |
| _Number of txs_ | 90 |
| _Avg. Confirmation Time (ms)_ | 41.0 |
| _P99_ | 77.5ms |
| _P95_ | 55.9ms |
| _P50_ | 40.6ms |
| _Tx validation time p50 (ms)_ | 10.9 |
| _End-to-end TPS_ | 72.71 tx/s |
| _Sustained TPS_ | 67.81 tx/s |
| _Backlog drain time (s)_ | 0.0 |
| _Snapshots observed_ | 61 |
| _Snapshots per second_ | 49.28 /s |
| _Avg txs per snapshot_ | 1.5 |
| _Peak node RSS (MB)_ | 158.5 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 4 |
      
