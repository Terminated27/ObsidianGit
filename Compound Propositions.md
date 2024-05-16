#computing #java

Compound propositions in Java refer to logical expressions that are formed by combining two or more simpler propositions using logical operators. These logical operators allow us to perform operations such as conjunction (AND), disjunction (OR), negation (NOT), and [[implication]] (IF-THEN). Understanding compound propositions is crucial in Java advanced programming as it enables developers to make decisions based on multiple conditions.

## Logical Operators

Java provides three main logical operators for combining propositions:

1. **Conjunction (`&&`)**: The conjunction operator returns `true` if both of the propositions being combined are true; otherwise, it returns `false`. It is represented by the double ampersand (`&&`) symbol.

    ```java
    boolean proposition1 = true;
    boolean proposition2 = false;
    boolean result = proposition1 && proposition2; // false
    ```

2. **Disjunction (`||`)**: The disjunction operator returns `true` if at least one of the propositions being combined is true; otherwise, it returns `false`. It is represented by the double vertical bar (`||`) symbol.

    ```java
    boolean proposition1 = true;
    boolean proposition2 = false;
    boolean result = proposition1 || proposition2; // true
    ```

3. **Negation (`!`)**: The negation operator reverses the truth value of a single proposition. If the original proposition is `true`, negation makes it `false`, and vice versa. It is represented by the exclamation mark (`!`) symbol.

    ```java
    boolean proposition = true;
    boolean result = !proposition; // false
    ```

## Compound Propositions Examples

### Example 1: Conjunction

Suppose we want to check if a number is both positive and even:

```java
int number = 6;
boolean isPositive = number > 0;
boolean isEven = number % 2 == 0;
boolean result = isPositive && isEven; // true
```

In this example, `isPositive` evaluates to `true` because `number` is greater than 0, and `isEven` evaluates to `true` because the remainder of dividing `number` by 2 is 0. Therefore, the conjunction of these two propositions (`isPositive && isEven`) results in `true`.
Just `&` will evaluate both arguments, `&&` evaluates only the second argument if the first is true too

### Example 2: Disjunction

Let's consider a scenario where we want to determine if a student has passed either the midterm or the final exam:

```java
double midtermScore = 75.5;
double finalScore = 80.0;
double passingScore = 60.0;

boolean passedMidterm = midtermScore >= passingScore;
boolean passedFinal = finalScore >= passingScore;
boolean result = passedMidterm || passedFinal; // true
```

In this example, both `passedMidterm` and `passedFinal` evaluate to `true` because the scores (`midtermScore`, `finalScore`) are greater than or equal to the passing score (`passingScore`). Therefore, the disjunction of these two propositions (`passedMidterm || passedFinal`) results in `true`.

### Example 3: Negation

Consider a situation where we want to check if a user does not have admin privileges:

```java
boolean hasAdminPrivileges = false;
boolean result = !hasAdminPrivileges; // true
```

In this example, since `hasAdminPrivileges` is initially set to `false`, applying negation (`!hasAdminPrivileges`) results in `true`.

## Key Concepts and Keywords

- Compound propositions: Logical expressions formed by combining simpler propositions using logical operators.
- Conjunction: Combining propositions using the logical AND operator (`&&`).
- Disjunction: Combining propositions using the logical OR operator (`||`).
- Negation: Reversing the truth value of a proposition using the logical NOT operator (`!`).

Remember to use these logical operators wisely when dealing with complex conditions in Java programming.

