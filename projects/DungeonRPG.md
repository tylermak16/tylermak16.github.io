---
layout: project
type: project
image: img/campfire.jpg
title: "DungeonRPG"
date: 2022-04-01
published: true
labels:
  - Java
summary: "I developed a turn based rpg dungeoning game with procedurally generated encounters with difficulty scaling with your level. This game requires you to manage your resources and judging when you should take a risky move or to fall back and live another day."
---

DungeonRPG was a project for AP Computer Science A with the goal of getting us familiar with creating programs that rely on user input from the console. Some additional features I added to my RPG include a party system, different character classes and abilities, various status afflictions, and multiple bosses. 

DunegeonRPG was the biggest project I've single handedly coded so far, with the main class alone having over 700 lines of code. Creating a game on this scale forced me to think about how to compartmentalize blocks of code and think of how the overall game would be structured when I added features and alter blocks of code that are all interlinked. For example, I had to utilize interfaces to create different types of hero classes and enemies each with their own movesets and stats. I also had to worry much more about scope due to how many layers of conditional statements and loops were needed.

Here is a chunk of codethat shows a failed attempt at escaping an enemy encounter:

```cpp
System.out.println("Escape attempt failed! Your opponent punishes you.");
                        mobs[mobsTurn].attack(party[turn]);
                        if(attackFormation[turn].getHealth()>0){
                            input = 0;
                        } else if(attackFormation[turn].getHealth() <= 0 && attackFormation[turn].getLastStand() == true){
                            if (attackFormation[turn].getHealth() <= 0 && attackFormation[turn].getLastStand() == true){
                                attackFormation[turn].setHealth(1);
                                if(Math.random()<=0.5){
                                    attackFormation[turn].setLastStand(false);
                                    System.out.println("The next hit to " + attackFormation[turn].getName() + " will be fatal");
                                } else {
                                System.out.println(attackFormation[turn].getName() + " is near death's door. The next time they take damage could be fatal");
                                }
```


