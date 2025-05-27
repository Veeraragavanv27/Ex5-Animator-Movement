# Ex5-Animator-Movement

## Aim :

To develop a animator movement for a player using unity.

## Algorithm :

## Step 1 : 

Import necessary models.

## Step 2 : 

 Right-click -> Create -> Animator Controller.

## Step 3 : 

Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4 : 

Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5 : 

Drag Animator Controller to the GameObject in the Inspector.

## Program :

### DEVELOPED BY : ALLEN JOVETH P
### REG NO : 212223240007

## PlayerController:


```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Movement : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;
    // Start is called before the first frame update
    void Start()
    {
        animator = this.gameObject.GetComponent <Animator>();
    }

    // Update is called once per frame
    void Update()
    {
        InputX = Input.GetAxis("Horizontal");
        animator.SetFloat("InputX", InputX);
        InputY = Input.GetAxis("Vertical");
        animator.SetFloat("InputY", InputY);
    }
}


```
## Output : 

![image](https://github.com/user-attachments/assets/ff3df604-7d96-41fc-9a33-11e5ecfaaf31)


![image](https://github.com/user-attachments/assets/cf362315-b157-4b95-a999-d5ff69dba125)


![image](https://github.com/user-attachments/assets/b5b4e7fc-9305-46d6-9390-fd6096b57dd8)


## Result :

Thus, An animator movement for a player using unity is developed successfully.
