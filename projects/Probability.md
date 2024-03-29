---
layout: project
type: project
image: img/stats.jpg
title: "Probability"
date: 2023
published: true
labels:
  - Java
summary: "An interface that allows the user to create their own statistical experiments/sample spaces, variables, and events to perform probabilistic calculations and operations."
---

This project was created during my free time while I was learning about permutations and combinations from discrete mathematics. The program prompts user input from the console to create or load a new experiment. The user can create events/variables as well as group them together. They would then be able to assign properties to them, such as the amount or probability and invoke operations to see what the outcome would be. This project is not finished as I plan to keep adding functionality and improving the user interface as I learn more about probablity and statistics. A big challenge in regards to the design of this project is how I am to go about the user interface. When creating programs that require user input, I typically only needed them to type to console. However, in this case there are too many elements and layers to instantiate sample spaces that it would be tedious and constrictive to have the user type everything in the console, so I am looking at looking how to implement GUI's.

Here is some code from my program showing some basic operations/calculations that can be used in experiments:
```cpp
private static int Factorial(int number) {
        int total = 1;
        while (number > 1) {
            total = total * number;
            number -= 1;
        }
        return total;
    }

    public static int Permutations(int set, int setGroup) {
        if (setGroup > set) {
            return 0;
        } else {
            return Factorial(set) / Factorial(set - setGroup);
        }
    }

    public static int Combinations(int set, int setGroup) {
        if (setGroup > set) {
            return 0;
        } else {
            return Factorial(set) / (Factorial(setGroup) * Factorial(set - setGroup));
        }
    }
```

