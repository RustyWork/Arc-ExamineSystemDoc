---
sidebar_position: 2
---
# InspectPoint Setup

---

:::tip[Reminder!!]

> After Setting up the **PointsManager**, we can setup up our **InspectPoint**. (Haven't set up the **PointsManager**. First setup that → [PointManager Setup](PointManagerSetup.md))

:::

---

## InspectPoint Prefab Setup

> You don't have to setup **Inspect Point** from start.

Just go inside **Arc ExamineSystem** folder → **Prefab** folder → **InspectPoint** folder and inside **InspectPoint** folder you will find prefab named <span style={{color: '#ff8011'}}>**InspectPoint**</span>, just drag that in your examinable object as a child.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\video15.mp4" type="video/mp4" />
  </video>
</div>
<br />

:::caution

**Inspect point** position or scale could be altered after adding it in examinable object so please set them accordingly.

:::

After that place the **Inspect Point** wherever you want on the examinable object.

And under **Inspect point** you will find a object named <span style={{color: '#ff8011'}}>**Visual**</span>.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\59.png)
</div>
<br />

- **Visual** → This holds the visual of the **Inspect point**.

---

## Setup

And when you click on **Inspect point** inside you will find a script named **Inspect Point**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\60.png)
</div>
<br />

### General 

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\61.png)
</div>
<br />

- **ShowInformation** → Enable it, if you want to show [Inspect panel](PointManagerSetup.md#general-settings) when you hover over **Inspect point**, you can disable it if you only want interaction with **Inspect Point**.

- **Information** → Add the information that you want to show.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\video33.mp4" type="video/mp4" />
  </video>
</div>
<br />
<p style={{color: '#888888', marginTop: '-1rem', textAlign: 'center'}}>Inspect Point Example</p>

- **WillFaceYou** → Enable it, if you want your **Inspect Point Visual** to look towards your camera. After enabling you will see this.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\62.png)
</div>
<br />

- **InspectPointVisual** → Here you have to add your **Visual** that is under **Inspect point**, adding parent in **InspectPointVisual** is highly discouraged.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\63.png)
</div>
<br />

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\video16.mp4" type="video/mp4" />
  </video>
</div>
<br />
<p style={{color: '#888888', marginTop: '-1rem', textAlign: 'center'}}>Cursor not visible because it was recorded using unity 
recorder</p>

---

### Interact Settings

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\64.png)
</div>
<br />

- **CanInteract** → Enable it, if you want to make the **Inspect Point** interactable.
- **OnClick** → Here you can add your custom **Event** to do customs things and this **OnClick** event is activated when you click on inspect point, it works similar as UI button.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\video34.mp4" type="video/mp4" />
  </video>
</div>
<br />

- **ObjectStateOnClick** → There are three options to choose, gets activated when you click on inspect point.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\65.png)
</div>
<br />

|Options | Description|
|--------|------------|
| **None** | Does nothing.|
| **Destroy** | Destroys the **Inspect point** on click.|
| **Hide** | Hides the **Inspect point** on click, but gets activated every time you re-enter in examine state.|

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\video17.mp4" type="video/mp4" />
  </video>
</div>
<br />

:::danger[Must Do.]

Please add **EventSystem** if not already in scene and Ensure **Physics RayCaster** is present in **ExamineOverlayCamera**.

:::

After that you will see one option named **HaveSound**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\66.png)
</div>
<br />

- **HaveSound** → Enable it, if you want to have sound in this inspect point.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\67.png)
</div>
<br />

Click on **Add InspectSound** to add **InspectSound** script, After clicking it will add a new script in inspect point object.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\2026-05-10 10-31-45-97.mp4" type="video/mp4" />
  </video>
</div>
<br />

:::tip[Learn More]

**Inspect Sound** is explained here → [InspectSound Setup](@site/docs/Arc%20Examine%20System%20Setup/Examinable%20Setups/InspectSoundSetup.md).

:::

---

## Visual Object Under Inspect Point Explained

As you know there is a **Visual** object under **Inspect Point**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\59.png)
</div>
<br />

This **Visual** is just a **Sprite Renderer** component you can customize it however you want.

---

:::danger[More information about **Inspect point**.]

There is **Sphere Collider** inside the inspect point you can change the radius to increase the area for interaction.

Make sure this **Sphere Collider** is not interfering with other colliders.

:::

:::important

Ensure they are added in **Inspect Points** list in **Examinable Object**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\43.png)
</div>
<br />

For all details [Examinables](@site/docs/Arc%20Examine%20System%20Setup/Examinable%20Setups/ExaminableSetup.md).

:::

<span style={{fontSize: '22px'}}>**Done..✨**</span>