# CSS Flexbox & Grid Guide

## Introduction
This guide covers the basics of **CSS Flexbox** and **CSS Grid**, two powerful layout techniques in modern web development.

## 1. CSS Flexbox
Flexbox (Flexible Box Layout) is used to create **one-dimensional layouts**, either in a row or column.

### **Basic Flexbox Example**
```css
.container {
  display: flex; /* Enables flexbox */
  justify-content: center; /* Aligns items horizontally */
  align-items: center; /* Aligns items vertically */
  gap: 10px; /* Adds space between items */
}

.item {
  width: 100px;
  height: 100px;
  background-color: lightblue;
}
```

### **Common Flexbox Properties**
| Property | Description |
|----------|------------|
| `display: flex` | Enables flexbox on a container |
| `flex-direction` | Defines the direction (row, column) |
| `justify-content` | Aligns items along the main axis |
| `align-items` | Aligns items along the cross axis |
| `gap` | Adds space between items |

---

## 2. CSS Grid
CSS Grid is a **two-dimensional layout system** that allows control over both rows and columns.

### **Basic Grid Example**
```css
.container {
  display: grid; /* Enables grid */
  grid-template-columns: repeat(3, 1fr); /* Three equal columns */
  gap: 10px; /* Space between grid items */
}

.item {
  width: 100px;
  height: 100px;
  background-color: lightcoral;
}
```

### **Common Grid Properties**
| Property | Description |
|----------|------------|
| `display: grid` | Enables grid layout |
| `grid-template-columns` | Defines column structure |
| `grid-template-rows` | Defines row structure |
| `gap` | Adds space between grid items |
| `justify-items` | Aligns items horizontally inside grid cells |
| `align-items` | Aligns items vertically inside grid cells |

---

## When to Use Flexbox vs. Grid
| Use Case | Recommended Method |
|----------|--------------------|
| One-dimensional layouts (row or column) | **Flexbox** |
| Two-dimensional layouts (rows & columns) | **Grid** |
| Centering elements | **Flexbox** |
| Complex page layouts | **Grid** |

### **Conclusion**
Both Flexbox and Grid are essential tools for modern CSS layouts. Use **Flexbox** for simpler, single-axis layouts and **Grid** for more complex, multi-axis designs.

Happy coding! 🎨🚀

