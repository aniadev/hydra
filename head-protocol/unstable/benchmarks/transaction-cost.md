--- 
sidebar_label: 'Transaction costs' 
sidebar_position: 3 
--- 

# Transaction costs 

Sizes and execution budgets for Hydra protocol transactions. Note that unlisted parameters are currently using `arbitrary` values and results are not fully deterministic and comparable to previous runs.

| Metadata | |
| :--- | :--- |
| _Generated at_ | 2026-07-23 06:50:34.736881655 UTC |
| _Max. memory units_ | 14000000 |
| _Max. CPU units_ | 10000000000 |
| _Max. tx size (kB)_ | 16384 |

## Script summary

| Name   | Hash | Size (Bytes) 
| :----- | :--- | -----------: 
| νHead | 2b91a7e666575a2465b8c7f6a7f960d5870cf13694a67f3215e014c5 | 12511 | 
| μHead | f2620ca915623f152a9d966b32364c416d31e1b3874065c3eaee999b* | 4856 | 
| νDeposit | c78e8c9205721eb3ef4410f3db9c6169fa6db497c24641d29c20529c | 1615 | 
| νCRS | 09db7ee6cf7a4b358dd5c8a2f19d2c048336ffc5a01ef35a47ca7072 | 2736 | 

* The minting policy hash is only usable for comparison. As the script is parameterized, the actual script is unique per head.

## `Init` transaction costs

| Parties | Tx size | % max Mem | % max CPU | Min fee ₳ |
| :------ | ------: | --------: | --------: | --------: |
| 1| 5352 | 8.65 | 2.84 | 0.48 |
| 2| 5448 | 9.53 | 3.13 | 0.49 |
| 3| 5543 | 9.92 | 3.25 | 0.50 |
| 5| 5736 | 11.03 | 3.61 | 0.52 |
| 10| 6218 | 13.37 | 4.35 | 0.56 |
| 50| 10058 | 34.83 | 11.07 | 0.95 |
| 100| 14858 | 61.65 | 19.47 | 1.44 |
| 115| 16296 | 69.61 | 21.96 | 1.59 |


## Cost of Increment Transaction

| Parties | Tx size | % max Mem | % max CPU | Min fee ₳ |
| :------ | ------: | --------: | --------: | --------: |
| 1| 2312 | 18.65 | 6.72 | 0.45 |
| 2| 2443 | 19.47 | 7.65 | 0.47 |
| 3| 2573 | 20.46 | 8.63 | 0.49 |
| 5| 2836 | 22.89 | 10.75 | 0.54 |
| 10| 3492 | 27.60 | 15.59 | 0.64 |
| 50| 8732 | 67.38 | 54.73 | 1.47 |
| 75| 12007 | 92.70 | 79.35 | 2.00 |


## Cost of Decrement Transaction

| Parties | Tx size | % max Mem | % max CPU | Min fee ₳ |
| :------ | ------: | --------: | --------: | --------: |
| 1| 633 | 16.44 | 6.04 | 0.35 |
| 2| 764 | 17.36 | 7.00 | 0.37 |
| 3| 895 | 18.26 | 7.96 | 0.39 |
| 5| 1158 | 20.09 | 9.87 | 0.43 |
| 10| 1814 | 24.58 | 14.64 | 0.53 |
| 50| 7054 | 63.25 | 53.42 | 1.36 |
| 75| 10328 | 87.70 | 77.73 | 1.87 |


## `Close` transaction costs

| Parties | Tx size | % max Mem | % max CPU | Min fee ₳ |
| :------ | ------: | --------: | --------: | --------: |
| 1| 660 | 15.62 | 10.46 | 0.38 |
| 2| 791 | 16.55 | 11.42 | 0.40 |
| 10| 1844 | 23.90 | 19.11 | 0.56 |
| 50| 7077 | 63.37 | 58.21 | 1.39 |
| 75| 10356 | 87.32 | 82.45 | 1.91 |


## `Contest` transaction costs

| Parties | Tx size | % max Mem | % max CPU | Min fee ₳ |
| :------ | ------: | --------: | --------: | --------: |
| 1| 691 | 18.93 | 13.57 | 0.43 |
| 2| 819 | 20.04 | 14.59 | 0.45 |
| 3| 949 | 21.13 | 15.60 | 0.48 |
| 5| 1213 | 23.28 | 17.62 | 0.52 |
| 10| 1875 | 28.66 | 22.66 | 0.63 |
| 50| 7113 | 74.76 | 63.73 | 1.53 |
| 71| 9863 | 98.13 | 85.06 | 1.99 |


## `FanOut` transaction costs
Involves spending head output and burning head tokens. Uses ada-only UTXO for better comparability.

| Parties | UTxO  | UTxO (bytes) | Tx size | % max Mem | % max CPU | Min fee ₳ |
| :------ | :---- | :----------- | ------: | --------: | --------: | --------: |
| 10 | 0 | 0 | 5529 | 23.24 | 42.86 | 0.89 |
| 10 | 1 | 57 | 5563 | 25.58 | 45.37 | 0.93 |
| 10 | 5 | 284 | 5698 | 35.83 | 55.69 | 1.09 |
| 10 | 10 | 569 | 5868 | 49.84 | 68.98 | 1.31 |
| 10 | 20 | 1137 | 6206 | 82.37 | 96.95 | 1.79 |
| 10 | 20 | 1139 | 6209 | 82.37 | 96.96 | 1.79 |


## `PartialFanOut` transaction costs
Largest chunk of ada-only outputs that can be distributed in one partial fanout step, computed dynamically. The last row is the maximum total UTxO count where at least one output can still be distributed.

| Distributed | UTxO (bytes) | Tx size | % max Mem | % max CPU | Min fee ₳ |
| ----------: | -----------: | ------: | --------: | --------: | --------: |
| 11 | 570 | 987 | 34.86 | 66.32 | 0.95 |
| 25 | 1311 | 1426 | 68.19 | 99.38 | 1.48 |
| 30 | 1308 | 1427 | 68.19 | 99.38 | 1.48 |
| 40 | 1309 | 1424 | 68.19 | 99.38 | 1.48 |
| 50 | 1308 | 1427 | 68.19 | 99.38 | 1.48 |
| 100 | 1311 | 1430 | 68.19 | 99.38 | 1.48 |
| 150 | 1307 | 1426 | 68.19 | 99.38 | 1.48 |
| 200 | 1309 | 1428 | 68.19 | 99.38 | 1.48 |
| 200 | 1308 | 1427 | 68.19 | 99.38 | 1.48 |


## `PartialFanOut` transaction costs (with native tokens)
Largest chunk of native-token outputs that can be distributed in one partial fanout step, computed dynamically. The last row is the maximum total UTxO count where at least one output can still be distributed.

| Distributed | UTxO (bytes) | Tx size | % max Mem | % max CPU | Min fee ₳ |
| ----------: | -----------: | ------: | --------: | --------: | --------: |
| 11 | 1130 | 1620 | 41.93 | 68.86 | 1.06 |
| 25 | 2268 | 2518 | 76.54 | 99.16 | 1.59 |
| 30 | 2037 | 2280 | 76.54 | 99.11 | 1.58 |
| 40 | 2226 | 2474 | 76.52 | 99.15 | 1.59 |
| 50 | 1974 | 2215 | 76.54 | 99.10 | 1.58 |
| 100 | 1974 | 2215 | 76.54 | 99.10 | 1.58 |
| 150 | 1995 | 2237 | 76.52 | 99.09 | 1.58 |
| 200 | 2415 | 2677 | 76.54 | 99.21 | 1.60 |
| 200 | 2499 | 2765 | 76.54 | 99.25 | 1.61 |


## `FinalPartialFanOut` transaction costs (with native tokens)
Terminal partial fanout step (FanoutProgress → Final) with outputs carrying a native token. Burns all head tokens and proves accumulator exhaustion via BLS proof.

| Distributed | UTxO (bytes) | Tx size | % max Mem | % max CPU | Min fee ₳ |
| ----------: | -----------: | ------: | --------: | --------: | --------: |
| 1 | 113 | 5417 | 21.97 | 44.27 | 0.89 |
| 5 | 540 | 5761 | 35.70 | 55.83 | 1.09 |
| 10 | 970 | 6085 | 53.90 | 70.60 | 1.36 |
| 10 | 1230 | 6346 | 53.78 | 70.64 | 1.37 |

