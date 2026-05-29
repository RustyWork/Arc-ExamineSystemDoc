---
sidebar_position: 5
---
# 🎮 Input Manager Setup

> <span style={{color: '#888888'}}> This is how you can easily setup your input manager </span>

---

## Overview

If you look under **ExamineManager** you will see <span style={{color: '#ff8011'}}>**Input Manager**</span> from here all inputs are managed.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\27.png)
</div>
<br />

:::note

You should have **Input System** package in your scene, it is already included in newer version of unity.

:::

---

## Input System Overview

If you look under **Arc Examine System** folder → **InputSystem** folder in that folder you will find one input system named <span style={{color: '#ff8011'}}>**ExamineInputSystem**</span>.

<br />

<div style={{textAlign: 'center'}}>
![Alt text](\img\28.png)
</div>

<p style={{color: '#888888', marginTop: '-1rem', textAlign: 'center'}}>The highlighted prefab</p>
<br />

All **Input Actions** are present here, and you can change all examine system inputs here.

<br />

<div style={{textAlign: 'center'}}>
![Alt text](\img\29.png)
</div>
<br />

:::tip[Note.]

All required inputs actions are already present here, you just need to adjust them as you like.

:::

---

## Explaining Input Manager script

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\27.png)
</div>
<br />

You can drag and drop your actions from **InputSystem** folder from **ExamineInputSystem** by clicking on little arrow on it.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Arc-ExamineSystemDoc/Videos/Video3.mp4" type="video/mp4" />
  </video>
</div>

### Script Properties

- **InputSystem** → Here you have to drag your **ExamineInputSystem**.
- **InteractAction** → This action lets you interact with examinable like entering and exiting examine state. [Default Key: [E]]

---

- **DifferentExitAction** → As **InteractAction**
handles entering and exiting of examine state, Enable **DifferentExitAction** if you don't want to use **InteractAction** as **examine state** exit action.

If you enable it you will see another field named **ExitAction**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\30.png)
</div>
<br />

- **ExitAction** → This action will lets you exit examine state. [Default Key : [Esc]]

---

- **RotateHoldAction** → Hold the **RotateHoldAction** to start examinable object rotation, releasing it will stop the rotation. [Default Key: [Mouse Left Button]]

- **RotateAction** → This is the action the rotates the examinable object and **RotateHoldAction** is the action that you have to hold in order to rotate. [Default: [Mouse Delta position]]

- **Scroll** → This action lets you **Zoom IN&Out**. [Default: [Mouse Scroll]]

#### All action are in there the correct field already, but in any case this is the correct order to place them.

<br />

<div style={{textAlign: 'center'}}>
![Alt text](\img\27.png)
</div>

<br />

And if using **DifferentExitAction**

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\30.png)
</div>
<br />

And a **Player Input** component should be present in object.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\32.png)
</div>
<br />
And in **Actions** field add your **ExamineInputSystem** object.


---

<span style={{fontSize: '22px'}}>**Done...✨**</span>