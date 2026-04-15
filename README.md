# Leap Year Checker (Kotlin)

This project contains a Kotlin program to determine whether a given year is a leap year based on the Gregorian calendar rules.

## 📘 Problem Statement

An extra day (February 29) is added every four years to correct the calendar since Earth takes approximately 365.25 days to orbit the Sun. This extra day creates a leap year.

A year is considered a leap year if it satisfies the following conditions:

1. The year must be divisible by 4
2. If divisible by 100, it is NOT a leap year
3. Unless it is also divisible by 400, then it IS a leap year

## ✅ Leap Year Logic

A year is a leap year if:

(year % 4 == 0 AND year % 100 != 0) OR (year % 400 == 0)

## 💻 Program Implementation (Kotlin)

```kotlin
import java.io.*
import java.util.*

fun main(args: Array<String>) {

    val year = readLine()!!.toInt()

    if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {
        println("True")
    } else {
        println("False")
    }

}
