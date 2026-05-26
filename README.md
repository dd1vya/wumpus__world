<h1>ExpNo 9: Solve Wumpus World Problem using Python demonstrating Inferences from Propositional Logic</h1> 
<h3>Name:DIVYADARSHINI M </h3>
<h3>Register Number:212224060072</h3>
<H3>Aim:</H3>
<p>
    To solve  Wumpus World Problem using Python demonstrating Inferences from Propositional Logic
</p>
<h1>Problem Description</h1>
<hr>
<h2>Wumpus World</h2>
<hr>
The Wumpus world is a simple world example to illustrate the worth of a knowledge-based agent and to represent knowledge representation.

The figure below shows a Wumpus world containing one pit and one Wumpus. There is an agent in room [1,1]. The goal of the agent is to exit the Wumpus world alive. The agent can exit the Wumpus world by reaching room [4,4]. The wumpus world contains exactly one Wumpus and one pit. There will be a breeze in the rooms adjacent to the pit, and there will be a stench in the rooms adjacent to Wumpus.

![image](https://github.com/natsaravanan/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/87870499/cd6b68dc-c79f-4dcb-8126-04da90d65912)

<center>Wumpus World Representation</center>
<p>
This is a python program that uses propositional logic sentences to check which rooms are safe. 

It is assumed that there will always be a safe path that the agent can take to exit the Wumpus world. The logical agent can take four actions: Up, Down, Left and Right. These actions help the agent move from one room to an adjacent room. The agent can perceive two things: Breeze and Stench.
</p>

<hr>
<h1>Sample Input and Output:</h1>
<hr>

![image](https://github.com/natsaravanan/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/87870499/8696111a-a4a7-47cb-ba4b-43a4ef88573f)
![image](https://github.com/natsaravanan/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/87870499/4be5bf06-79fa-4fa0-9334-38a33f06060b)

<hr>
<h3>Program:</h3>

```
room={
(0,1):"Breeze",
(1,1):"Save",
(2,1):"GOLD"
}

x=y=0
score=0

while True:

    print("\npress u to move up")
    print("press d to move down")
    print("press l to move left")
    print("press r to move right")

    m=input()

    if m=="u":x-=1
    if m=="d":x+=1
    if m=="l":y-=1
    if m=="r":y+=1

    if (x,y) in room:

        print("\ncurrent location:",room[(x,y)])

        if room[(x,y)]=="GOLD":
            score=1000
            print("\nGOLD FOUND!You won....")
            print("Your score is:",score)
            break
```
<h3>Output:</h3>

<img width="384" height="620" alt="image" src="https://github.com/user-attachments/assets/b646502b-43ce-4ed9-aefc-015290f42244" />

<hr>
<h3>Result:</h3>

Wumpus World Problem using Python demonstrating Inferences from Propositional Logic was solved.
