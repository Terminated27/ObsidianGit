On input 0, the machine goes from state i to state 2i%12. On input 1, the machine goes from state i to state (2i + 1)%12.

| States | Input transition 0 | Input Transition 1 |
| ------ | ------------------ | ------------------ |
| 0      | 0                  | 1                  |
| 1      | 2                  | 3                  |
| 2      | 4                  | 5                  |
| 3      | 6                  | 7                  |
| 4      | 8                  | 9                  |
| 5      | 10                 | 11                 |
| 6      | 0                  | 1                  |
| 7      | 2                  | 3                  |
| 8      | 4                  | 5                  |
| 9      | 6                  | 7                  |
| 10     | 8                  | 9                  |
| 11     | 10                 | 11                 |
6 equivalent states {0,6}{1,7}{2,8}{3,9}{4,10}{5,11}

```mermaid
graph TD;
	0,6-->|0|0,6;
	0,6-->|1|1,7;
	1,7-->|0|2,8;
	1,7-->|1|3,9;
	2,8-->|0|4,10;
	2,8-->|1|5,11;
	3,9-->|0|0,6;
	3,9-->|1|1,7;
	4,10-->|0|2,8;
	4,10-->|1|3,9;
	5,11-->|0|4,10;
	5,11-->|1|5,11;
```
```mermaid
graph LR;
	start --> 0
	0 --> |a|1
	1 --> |b|2
```
```mermaid
graph LR;
	start --> 0
	0 --> |a|1
	0 --> |lambda|1
	1 --> |b|2
	1 --> |lambda|2
```
