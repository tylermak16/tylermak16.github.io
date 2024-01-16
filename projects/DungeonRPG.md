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

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

DungeonRPG was a project for AP Computer Science A with the goal of getting us familiar with creating programs that rely on user input from the console. Some additional features I added to my RPG include a party system, different character classes and abilities, various status afflictions, and multiple bosses. 

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

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
