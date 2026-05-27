---
sidebar_position: 4
---

# ❌ Player Disable

> **Now, when we are in the examine state, we don't want our player to interfere. Here is how you can disable your player while in the examine state.**

---

To disable any block of code use this syntax: ⇩

```csharp

if (!ExamineManager.instance.ReadState_isOccupied)
{
    //Code that you want to disable.
}

```

Example:

I used it to disable my player while in examine state.

<br />

<div style={{textAlign: 'center'}}>
![Alt text](\img\31.png)
</div>

<br />

Now, when we enter the examine state, that block of code gets disabled and stays disabled till we exit the examine state.

---

> <span style={{fontSize: '22px'}}>**You can disable code by using this method as well..**</span>

<br />

We are going to do this by using **ExamineManager** events.

<br />

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\Video4.mp4" type="video/mp4" />
  </video>
</div>

<br />

:::note

Recommended disabling any code that interferes while in examine state.

:::

<span style={{fontSize: '22px'}}>**Done..🎉**</span>