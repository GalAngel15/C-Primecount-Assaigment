# C-Primecount-Assaigment

## Prime Number Finder

This software is designed to find prime numbers within a specified range using the C programming language. The program utilizes the `fork` system call to create multiple child processes that work in parallel and share memory to find the prime numbers.

### Usage

The program takes input of lower and upper bounds (`lval` and `uval`) and displays all the prime numbers within that range. You can provide the bounds using the `-l` and `-u` parameters, respectively. For example:

```
./prime_finder -l 1 -u 100
```

### Key Features

- Prime Number Identification: The program searches and identifies prime numbers within the specified range defined by the `lval` and `uval` bounds.
- Use of `fork` System Call: The program creates multiple child processes using the `fork` system call to enable parallel processing of prime numbers.
- Shared Memory Usage: The program utilizes shared memory using the `mmap` function to share data between the child and parent processes.
- Concurrent Processing: The child processes work concurrently to find the prime numbers in the range, resulting in faster processing.

### Compilation Instructions

To compile the program, use a C compiler compatible with the C language, for example:

```
gcc -o prime_finder prime_finder.c -lm
```

# README

## מוצא מספרים ראשוניים

תוכנה זו מיועדת למציאת מספרים ראשוניים בתחום מסוים בעזרת שפת התכנות C. התוכנה משתמשת בשיחת המערכת `fork` על מנת ליצור תהליכים ילדים מרובים שעובדים במקביל ומשתמשים בזכרון משותף למציאת המספרים הראשוניים.

### שימוש

התוכנה מקבלת כקלט גבולות תחום (`lval` ו- `uval`) ומציגה את כל המספרים הראשוניים בין הגבולות הללו. תוכל לספק את הגבולות באמצעות הפרמטרים `-l` ו- `-u` בהתאמה. לדוגמה:

```
./prime_finder -l 1 -u 100
```

### תכונות עיקריות

- מציאת מספרים ראשוניים: התוכנה מחפשת ומוצאת מספרים ראשוניים בתחום המוגדר על ידי הגבולות `lval` ו- `uval`.
- שימוש בקריאת המערכת `fork`: התוכנה יוצרת תהליכים "ילדים" מרובים באמצעות `fork` על מנת לאפשר עבודה במקביל של חיפוש המספרים הראשוניים.
- שימוש בזכרון משותף: התוכנה משתמשת בזכרון משותף באמצעות הפונקציה `mmap` כדי לשתף מידע בין התהליכים "הילדים" והורה.
- עבודה בו זמנית: התהליכים עובדים במקביל לאיתור המספרים הראשוניים בתחום, מה שמאפשר עיבוד מהיר יותר.
