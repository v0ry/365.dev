---
id: Data Types
aliases: 
tags: 
created: 2025-04-14T05:56
lead: +++ Lead paragraph goes here +++
modified: 2025-04-15T17:45
status: TODO
template-version: "2"
template_type: Course Note
uuid: <% tp.user.uuid() %>
---
# C Data Types

> [!Summary]
> `= this.lead` 

#  [C Data Types](https://www.w3schools.com/c/c_data_types.php)
| Data Type | Size         | Description                                                                                           | Example |
| --------- | ------------ | ----------------------------------------------------------------------------------------------------- | ------- |
| `int`     | 2 or 4 bytes | Stores whole numbers, without decimals                                                                | `1`     |
| `float`   | 4 bytes      | Stores fractional numbers, containing one or more decimals. Sufficient for storing 6-7 decimal digits | `1.99`  |
| `double`  | 8 bytes      | Stores fractional numbers, containing one or more decimals. Sufficient for storing 15 decimal digits  | `1.99`  |
| `char`    | 1 byte       | Stores a single character/letter/number, or ASCII values                                              | `'A'`   |

# C Character Data Types
The character must be surrounded by single quotes, like 'A' or 'c', and we use the `%c` format specifier to print it

You can use ASCII values to display certain characters.
```c
#include <stdio.h>

int main(void)
{
  char c;
  int i;
  printf("Insert character: ");
  scanf(" %c", &c);

  printf("Number: %i\n", c);
  printf("ASCII Character: %c\n", c);

  printf("-----------------------------\n");
  printf("Insert number: ");
  scanf(" %i", &i);

  printf("Number: %i\n", i);
  printf("ASCII Character: %c\n", i);
  return 0;
}

```

```bash
Insert character: a
Number: 97
ASCII Character: a
-----------------------------
Insert number: 97
Number: 97
ASCII Character: a
```

# C Numeric Data Types
Use `int` when you need to store a whole number without decimals, like 35 or 1000, and `float` or `double` when you need a floating point number (with decimals), like 9.99 or 3.14515.

# C Decimal Precision
 use a dot (`.`) followed by a number that specifies how many digits that should be shown after the decimal point

# C The sizeof Operator
Why Should I Know the Size of Data Types?
Using the right data type for the right purpose will **save memory** and **improve the performance** of your program.

# C Type Conversion
##  **Implicit Conversion** (automatically)  
Implicit conversion is done automatically by the compiler when you assign a value of one type to another. 
```c
float sum = 5 / 2;  
  
printf("%f", sum); // 2.000000
```
## **Explicit Conversion** (manually)
Explicit conversion is done manually by placing the type in parentheses `()` in front of the value.
```c
int num1 = 5;  
int num2 = 2;  
float sum = (float) num1 / num2;  
  
printf("%.1f", sum); // 2.5
```

# C Constants




---
## 

---

## **Practice Questions**
<!-- Flashcard style - Can be parsed by Obsidian plugins like Obsidian CardBoard or Obsidian Recall -->

| **Frage**                                                                    | **Antwort**                                          |
| ---------------------------------------------------------------------------- | ---------------------------------------------------- |
| Wie groß ist ein `unsigned int` in der Regel?                                | 4 Byte                                               |
| Welche Zahlen kann ein `unsigned int` enthalten?                             | positive Ganzzahlen                                  |
| Kann ein `unsigned int` negative Zahlen speichern?                           | nein                                                 |
| Was bedeutet es, dass `unsigned int` alle Zahlen im Bereich abbilden kann?   | alle Zahlen zwischen 0 und dem Maximalwert           |
| behandelt der Compiler Whitespace in Zeichenketten anders, als im Sourcecode | ja, Whitespace ist dort relevant und bleibt erhalten |
| Was ist `%` in C?                                                            | ein binärer Operator (Modulo)                        |
| Wie viele Operanden benötigt `%`?                                            | zwei (binär)                                         |
| Was berechnet `a % b`?                                                       | den Rest der Division von `a` durch `b`              |
| Was ist das Ergebnis von `10 % 3`?                                           | 1                                                    |
| Ist `%` für Gleitkommazahlen (`float`, `double`) erlaubt?                    | nein, nur für Ganzzahlen                             |
| Was ergibt `5 % 5`?                                                          | 0                                                    |
| Kann `%` mit negativen Zahlen verwendet werden?                              | ja, aber das Vorzeichen hängt vom Compiler ab        |
|Was ist das Ziel der strukturierten Programmierung?|klare, nachvollziehbare Programme ohne unkontrollierte Sprünge|
|Welche drei Grundstrukturen erlaubt strukturierte Programmierung?|Sequenz, Verzweigung, Wiederholung|




## **Code Output Questions**

```c
#include <stdio.h>
#include <stdint.h>

int main() {
    int8_t a = 0;
    a = a - 1;
    printf("%d", a);
    return 0;
}
```

`int8_t` ist ein **signed 8-bit Integer**.
    
Wertebereich: **-128 bis +127**
    
Du startest mit `a = 0`, dann machst du `a = a - 1;` → Ergebnis: **-1**

---


---

## ✅ Tasks
- [ ] 

---
