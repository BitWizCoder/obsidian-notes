Great question, Muhammad. Let’s clarify how the **Design System File (Step 1)** connects with the **Component Library File (Step 2)** — this is the **foundation of working efficiently in Figma across files**.

---

## 🔄 Relationship Between the Two Files

Think of it like this:

|Design System File|→|Component Library File|
|---|---|---|
|Defines the **visual rules** (colors, typography, spacing, etc.)|Uses those styles to build **reusable components**||

---

## 🗂️ FILE STRUCTURE OVERVIEW

You’ll be working with **2 linked Figma files**:

### 1. **Design System File** (`design-system.fig`)

- Defines **Color Styles**, **Text Styles**, **Effect Styles** (like shadows), **Grids**, and maybe **Icons**.
    
- Saved styles can be **published** and reused anywhere.
    

### 2. **Component Library File** (`components.fig`)

- Contains all the UI components like buttons, CTAs, cards, navbars, etc.
    
- This file will **import and use the styles** from `design-system.fig`.
    

---

## 🔧 How to Use Styles Across Files

### ✅ Step-by-Step: Linking Files

#### **Step 1: Create and Publish Styles in the Design System File**

1. Create your `design-system.fig`.
    
2. Define styles:
    
    - **Text Styles**: `Heading / H1`, `Body / Small`, etc.
        
    - **Color Styles**: `Primary / 500`, `Surface / Background`, `Text / Light`, etc.
        
    - **Effect Styles**: Drop shadows, inner shadows.
        
3. In the **Assets Panel**, go to `Library` and click **Publish Styles**.
    
    - This makes your styles available to other files.
        

---

#### **Step 2: Use Styles in the Component Library File**

1. Open your `components.fig` file.
    
2. Go to `Assets` → `Libraries` (book icon).
    
3. Enable the `design-system.fig` as a **linked library**.
    
4. Now, when creating buttons, navbars, or cards:
    
    - You’ll see the **text and color styles** from your design system.
        
    - Just apply them using the style menus in Figma.
        

> ✅ Example:  
> When designing a “Primary Button”, apply:
> 
> - Fill: `Primary / 500`
>     
> - Text: `Text / Button`
>     
> - Shadow: `Elevation / Medium`
>     

Now, if you ever **change your Primary color** in the Design System File, **it updates everywhere** it’s used (including in all components).

---

## 🔁 Bonus: What Happens When You Update Styles?

Let’s say you later decide to:

- Darken the `Primary / 500` color
    
- Or change the base font to Inter
    

You can do that **once** in `design-system.fig`, hit “Publish”, and then:

- In `components.fig` (and any other file using those styles), you’ll see a **“Review Changes” prompt**.
    
- You can then **accept changes**, and your whole system is updated.
    

---

## ✅ Why This Matters

- **Centralized control**: You don’t have to hunt through 20 components to change a color.
    
- **Design consistency**: All elements stay visually aligned.
    
- **Faster work**: You build once, use everywhere.
    

---

### Want a Quick Template?

I can create a mini Figma structure like this:

```
📁 design-system.fig
  🎨 Color Styles
  🅰️ Typography
  🌫️ Shadows

📁 components.fig
  🧱 Buttons
  🧱 Cards
  🧱 CTAs
  🧱 Navbars
```

