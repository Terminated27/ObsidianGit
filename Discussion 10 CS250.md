1. (\\''+L)*
2. $\lambda$ NFA
```mermaid
graph TD;
	start --> 1;
	1 -->|''| 2;
	2 -->|\| 3;
	2 -->|L| 4;
	2 -->|lambda| 4;
	3 -->|''| 4;
	4 -->|lambda| 2;
	4 -->|''| 5;
```
3. NFA
```mermaid
graph LR;
	start --> |empty set|3;
	start --> |empty set|0
	0 --> |L|1;
	0 --> |\|2;
	2 --> |''|3;
	1 --> |L|1;
	3 --> |L|1;
	3 --> |\|2;
	1 --> |\|2;

```
3. transition table:

| States | input L | input \ | input " | input emptyset |
| ------ | ------- | ------- | ------- | -------------- |
| start  |         |         |         | 0 or 3         |
| 0      | 1       | 2       |         |                |
| 1      | 1       | 2       |         |                |
| 2      |         |         | 3       |                |
| 3      | 1       | 2       |         |                |
|        |         |         |         |                |
4. NFA to DFA
```mermaid
graph TD;
	0 --> |L|1;
	0 --> |\|2;
	2 --> |''|3;
	1 --> |L|1;
	3 --> |L|1;
	3 --> |\|2;
	1 --> |\|2;
```
4. 
christian mugisha
