---
sidebar_position: 6
---

# 🧩 UI Setup

> Now we can setup our **UI** to display **Examinable** object name, description and more.

---

## Overview

Here we have to setup two things: **UI** and **Examine UI** script.

---

## UI Setup Explained

> First we have to setup **UI** before setting up the script.

Go under **ExamineManager-UI** object you will find an object named <span style={{color: '#ff8011'}}>**UI-Holder**</span>.  
**UI-Holder** holds all content such as **Name** (Text), **Description** (Text), examine state **Close Button**, and icons of input actions used in the examine system.

<br />

<div style={{display: 'flex', gap: '10px', alignItems: 'center'}}>
  <img src="/img/87.png" alt="UI Holder" width="50%" />
  <span style={{fontSize: '24px', flexShrink: 0}}>→</span>
  <img src="/img/88.png" alt="UI Holder Content" width="50%" />
</div>

<br />

:::note

All **UI** under **UI-Holder** is just placeholder content.  
You are free to customize it however you want.

:::

---

## Examine UI Script Setup

If you go under **ExamineManager**, you will find a component named **UI Manager**.  
Inside that object, you will find a script named **Examine UI**.

<br />

<div style={{display: 'flex', gap: '10px', alignItems: 'center'}}>
  <img src="/img/89.png" alt="UI Manager" width="50%" />
  <span style={{fontSize: '24px', flexShrink: 0}}>→</span>
  <img src="/img/90.png" alt="Examine UI Script" width="50%" />
</div>

<br />

### Explaining

> It time to understand **UI** script.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/90.png" alt="Examine UI Script" style={{width: '300px', height: 'auto'}} />
</div>

<br />

## <span style={{fontSize: '22px'}}>Reference</span>

<div style={{margin: '25px 0'}} />

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/94.png" alt="Reference Settings" />
</div>

<br />

- **ExamineManager** → Add your **ExamineManager** script reference here.

---

## <span style={{fontSize: '22px'}}>Hover Visual Settings</span>

<div style={{margin: '25px 0'}} />

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/95.png" alt="Hover Visual Settings" />
</div>

<br />

- **ShowVisualHint** → Enable it, if you want to have a visual that hints to you when you are hovering over your examinable object.

After you enable **ShowVisualHint**, a new field will show up named <span style={{color: '#ff8011'}}>**VisualHint**</span>.

Before I explain you **VisualHint**, if you go under **ExamineManager-UI** you will find an object named **HoverVisual**.

<br />

<div style={{display: 'flex', gap: '10px', alignItems: 'center'}}>
  <img src="/img/92.png" alt="HoverVisual Object" width="50%" />
  <span style={{fontSize: '24px', flexShrink: 0}}>→</span>
  <img src="/img/91.png" alt="HoverVisual Preview" width="50%" />
</div>

<br />

- **HoverVisual** → It is the object that contains your **HoverVisual** that gets displayed when you hover over the examinable object.

Time to understand <span style={{color: '#ff8011'}}>**VisualHint**</span>.

- **VisualHint** → Add the visual you want to show when you hover over the examinable object.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/93.png" alt="VisualHint" />
</div>

<br />

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Videos/video25.mp4" type="video/mp4" />
  </video>
</div>

<br />

---

## <span style={{fontSize: '22px'}}>UI Settings</span>

<div style={{margin: '25px 0'}} />

> Time for most interesting thing **UI** Setup

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/96.png" alt="UI Settings" />
</div>

<br />

- **HaveUI** → Enable it, if you want to show **UI** during your examine state.

:::tip[Note]

<p style={{color: '#ffffff', fontSize: '13px'}}>
Disabling <strong>HaveUI</strong> will not affect visibility of 
<a href="/Arc%20Examine%20System%20Setup/Examinable%20Setups/InspectPoints%20Setup/InspectPointsSetup">InspectPoint</a> 
and 
<a href="/Arc%20Examine%20System%20Setup/Examinable%20Setups/ItemInspect%20Setup/ItemInspectSetup">ItemInspect</a>.
</p>

:::

After you enable **HaveUI**, you will see few fields.

Lets talk about **UI Holder**, **ExaminableObject NameLabel** and **ExaminableObject DescriptionLabel** first.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/97.png" alt="UI Holder References" />
</div>

<br />

- **UI Holder** → Add the parent that holds all of your UI contents, like **NameLabel** for **ExaminableObject** and **DescriptionLabel** for **ExaminableObject** etc.  
<span style={{fontSize: '24px', flexShrink: 0}}>→</span> [Add the **UI-Holder** found under **ExamineManager-UI** object].

- **ExaminableObject NameLabel** → Add the **Text** here that will display the **Name** of your examinable object.  
<span style={{fontSize: '24px', flexShrink: 0}}>→</span> [Add the **Name** object found under **UI-Holder** object].

- **ExaminableObject DescriptionLabel** → Add the **Text** here that will display the **Description** of your examinable object.  
<span style={{fontSize: '24px', flexShrink: 0}}>→</span> [Add the **Description** object found under **UI-Holder** object].

<br />

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Videos/video26.mp4" type="video/mp4" />
  </video>
</div>

<br />

:::note

**UI-Holder** is already explained above. Look for [**UI Setup Explained**].

:::

Time to explain last two fields.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/img/98.png" alt="Visibility Settings" />
</div>

<br />

- **CanChangeVisibilityWhileExamining** → Enable it, if you want to control the visibility of your **UI** while in examine mode.

- **VisibilityInput** → To control your **UI** visibility while in examine mode, you must add an **Input Action**.  
<span style={{fontSize: '24px', flexShrink: 0}}>→</span> [Add inputAction named **ShowHideUIAction** here. **ShowHideUIAction** default key is [H], you can change it].

<br />

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Videos/video27.mp4" type="video/mp4" />
  </video>
</div>

<br />

And **UI** done.... ✨