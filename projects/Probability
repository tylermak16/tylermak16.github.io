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

This project was created during my free time while I was learning about permutations and combinations from discrete mathematics. The program prompts user input from the console to create or load a new experiment. The user can create events/variables as well as group them together. They would then be able to assign properties to them, such as the amount or probability and invoke operations to see what the outcome would be. This project is not finished as I plan to keep adding functionality and improving the user interface as I learn more about probablity and statistics.

Here is some code showing some basic operations/calculations that you can use in an experiment: 
```
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

