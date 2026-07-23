--- 
sidebar_label: 'End-to-end benchmarks' 
sidebar_position: 4 
--- 

# End-to-end benchmark results 

This page is intended to collect the latest end-to-end benchmark  results produced by Hydra's continuous integration (CI) system from  the latest `master` code.

:::caution

Please note that these results are approximate  as they are currently produced from limited cloud VMs and not controlled hardware.  Rather than focusing on the absolute results,   the emphasis should be on relative results,  such as how the timings for a scenario evolve as the code changes.

:::

_Generated at_  2026-07-23 06:53:31.32026181 UTC


## Baseline Scenario



| Number of nodes |  1 | 
| -- | -- |
| _Number of txs_ | 300 |
| _Avg. Confirmation Time (ms)_ | 480.1 |
| _P99_ | 495.1ms |
| _P95_ | 494.8ms |
| _P50_ | 483.0ms |
| _Tx validation time p50 (ms)_ | 338.6 |
| _End-to-end TPS_ | 598.87 tx/s |
| _Backlog drain time (s)_ | 0.5 |
| _Snapshots observed_ | 4 |
| _Snapshots per second_ | 7.98 /s |
| _Avg txs per snapshot_ | 75.0 |
| _Peak node RSS (MB)_ | 163.6 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 2 |
      

## Three local nodes



| Number of nodes |  3 | 
| -- | -- |
| _Number of txs_ | 900 |
| _Avg. Confirmation Time (ms)_ | 2414.1 |
| _P99_ | 2675.2ms |
| _P95_ | 2674.6ms |
| _P50_ | 2460.6ms |
| _Tx validation time p50 (ms)_ | 1271.9 |
| _End-to-end TPS_ | 335.55 tx/s |
| _Sustained TPS_ | 1281.93 tx/s |
| _Backlog drain time (s)_ | 2.6 |
| _Snapshots observed_ | 10 |
| _Snapshots per second_ | 3.73 /s |
| _Avg txs per snapshot_ | 90.0 |
| _Peak node RSS (MB)_ | 161.9 |
| _Number of Invalid txs_ | 0 |
| _Fanout outputs_        | 4 |
      
