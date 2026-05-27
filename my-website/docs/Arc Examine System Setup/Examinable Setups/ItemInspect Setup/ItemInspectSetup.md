# Item Inspect Setup

> Now if you want to **Interact** with an object while in examine mode, this component will help you.

---

## Overview

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Videos/video19.mp4" type="video/mp4" />
  </video>
</div>

<br />

<p style={{color: '#888888', marginTop: '-1rem', textAlign: 'center'}}>
Item Inspect example
</p>

:::info[What is Item Inspect?]

It is similar to **InspectPoint** but it offers more things specially made for **Item Interaction**.

:::

---

## Setup

Add the <span style={{color: '#ff8011'}}>**Item Interact**</span> Component to interact with an object in the examine state.

Once you add the component you will see this.

<br />

<div style={{display: 'flex', gap: '10px', alignItems: 'center'}}>
  <img src="/img/69.png" alt="Item Inspect Setup" width="50%" />
  <img src="/img/74.png" alt="Item Inspect Inspector" width="50%" />
</div>

<br />

---

## Explaining

> And now we can finally start the setup and it would be easier to understand as it is similar to **InspectPoint**.

---

## Interact Settings

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/71.png" alt="Interact Settings" />
</div>

<br />

- **OnClick** → Here you can add your custom **Methods** to do custom things, and this **OnClick** event is activated when you click on Item Inspect. It works similarly to a UI button.

- **ObjectStateOnClick** → There are three options to choose, gets activated when you clicked on Item Inspect.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/65.png" alt="Object State On Click" />
</div>

<br />

| Options | Description |
|----------|-------------|
| **None** | Does nothing. |
| **Destroy** | Destroys on click. |
| **Hide** | Hides on click, but gets activated every time you re-enter in examine state. |

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Videos/video17.mp4" type="video/mp4" />
  </video>
</div>

<br />

<p style={{color: '#888888', marginTop: '-1rem', textAlign: 'center'}}>
Cursor not visible because it was recorded using Unity Recorder
</p>

:::danger[Must Do.]

Please add **EventSystem** if not already in scene and ensure **Physics RayCaster** is present in **ExamineOverlayCamera**.

:::

After that you will see one option named **HaveSound**.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/66.png" alt="HaveSound" />
</div>

<br />

- **HaveSound** → Enable it, if you want to have sound in this Item Inspect.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/67.png" alt="InspectSound Setup" />
</div>

<br />

Click on **Add InspectSound** to add **InspectSound** script.  
After clicking it will add a new script in Item Inspect object.

:::tip[Learn More]

**Inspect Sound** is explained here → [InspectSound Setup](@site/docs/Arc%20Examine%20System%20Setup/Examinable%20Setups/InspectSoundSetup.md).

:::

---

## HighLight Settings

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/72.png" alt="Highlight Settings" />
</div>

<br />

- **ShowHighlight** → Enable it, if you want to show an emission highlight when the player hovers over the ItemInspect object with the mouse.
- **EmissiveColor** → You can control your emissive color from here.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Videos/video20.mp4" type="video/mp4" />
  </video>
</div>

<br />

- **Intensity** → Here you can control the intensity of your emissive color.

After that you will see an empty list of **Renderer Objects**.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/73.png" alt="Renderer Objects" />
</div>

<br />

Here you can add your objects on which you want to show the highlight.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Videos/Video21.mp4" type="video/mp4" />
  </video>
</div>

<br />

---

## AfterClickLabel Settings

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/75.png" alt="AfterClickLabel Settings" />
</div>

<br />

- **AfterClickLabel** → Enable it, if you want to show a label after you click on **ItemInspect**. It could be helpful if you want to indicate to the player with **Text** that something has happened after clicking on **ItemInspect**.  
Like — "**Object has added to inventory**".

After enabling **AfterClickLabel** you will see three properties.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/76.png" alt="AfterClickLabel Properties" />
</div>

<br />

- **Label** → Here add the **Text** that you want to show.
- **DurationState** → Here are two options that you can change.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/77.png" alt="DurationState" />
</div>

<br />

| Options | Description |
|----------|-------------|
| None | Does nothing. |
| Duration | Use it, if you want to show the **Label** for a limited time. |

And when you set **DurationState** to **Duration**, one more option will appear.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/78.png" alt="Duration" />
</div>

<br />

- **Duration** → Here you can select how long you want the label to stay.

---

> <span style={{fontSize: '20px'}}>But setup for **AfterClickLabel** is not yet completed.</span>

Lets setup **UI** for it.

---

## AfterClickLabel UI Setup

> Lets first look at **UI** for AfterClickLabel. If you go under **ExamineManager-UI** you will see an object named <span style={{color: '#ff8011'}}>**ItemPrompt-UIHolder**</span>

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/79.png" alt="ItemPrompt UI Holder" />
</div>

<br />

- **ItemPrompt-UIHolder** → It holds the content like **Background** and **Prompt(Text)**.

- **Background** → This is the object that acts as **Background** behind **Prompt(Text)**.

<br />

<div style={{display: 'flex', gap: '10px', alignItems: 'center'}}>
  <img src="/img/80.png" alt="Background Object" width="50%" />
  <span style={{fontSize: '24px', flexShrink: 0}}>→</span>
  <img src="/img/81.png" alt="Background Preview" width="50%" />
</div>

<br />

> <span style={{fontSize: '18px'}}>It is just an **Image** so customize it however you want.</span>

- **Prompt** → It is the **Text** that will display whatever you have written in **AfterClickLabel** in the **Label** field.

<br />

<div style={{display: 'flex', gap: '10px', alignItems: 'center'}}>
  <img src="/img/82.png" alt="Prompt Text" width="50%" />
  <span style={{fontSize: '24px', flexShrink: 0}}>→</span>
  <img src="/img/83.png" alt="Prompt Preview" width="50%" />
</div>

<br />

---

> <span style={{fontSize: '20px'}}>Now we only have to setup the **UI** script.</span>

## Item Inspect UI Manager Script Setup

> This is a very small script setup.

You will find an object named **Item Inspect UI Manager** under **ExamineManager** object.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/84.png" alt="Item Inspect UI Manager Object" />
</div>

<br />

In this object you will find a script named <span style={{color: '#ff8011'}}>**Item Inspect UI Manager**</span>.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/85.png" alt="Item Inspect UI Manager Script" />
</div>

<br />

- **UIHolder** → Add the object that holds the **UI** like **Background**, **Text**, and other content.
- **Label** → Add the text object that will display whatever you have written in **AfterClickLabel** in the **Label** field.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Videos/video22.mp4" type="video/mp4" />
  </video>
</div>

<br />

> **Done**...

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Videos/video23.mp4" type="video/mp4" />
  </video>
</div>

<br />

<p style={{color: '#888888', marginTop: '-1rem', textAlign: 'center'}}>
AfterClickLabel example
</p>

---

:::tip

If you want **InspectPoint** features in your **ItemInspect** object, just add the **InspectPoint** script where the **ItemInspect** script is present.  
Just do not forget to disable **Interact Settings** and **WillFaceYou** from the **InspectPoint** script, and now you are done.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/86.png" alt="InspectPoint Features" />
</div>

<br />

:::

:::tip[Helpful Feature]

If you want to change the text in the **Label** field to something else.

Just use this method. By the way, this method is present in the **Item Inspect** script.

```csharp
public void ChangeLabel(string newLabel)
{
   label = newLabel;
}