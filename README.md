# EXP06 Book Cover Design using HTML & CSS

### DATE : 16/10/2025

##  AIM:
To design a simple and visually appealing Book Cover using HTML and CSS.



##  DESIGN STEPS:

### Step 1:
Create a new project folder and include the files `index.html` and `styles.css`.

### Step 2:
Build the basic HTML structure for the book cover using:
- `<div>` containers  
- `<h1>`, `<h3>` for title & author  
- Images or shapes (optional)

### Step 3:
Apply CSS styling to create a professional book-cover effect using:
- Background colors / gradients  
- Borders & shadows  
- Font styling  
- Flexbox for alignment

### Step 4:
Adjust spacing, padding, and font sizes to ensure visual balance.

### Step 5:
Preview the final output in a web browser.

##  PROGRAM:
```
Developed By : Krishna Prasad S
Register No. : 212223230108
```

### index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Book Cover - The Silent Shore</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <div class="cover">
    <div class="cover-inner">
      <h1 class="title">The Silent Shore</h1>
      <h2 class="subtitle">A Novel by Someone</h2>
      <p class="tag">A story of tides, time and tiny rebellions.</p>
      <div class="spine">The Silent Shore</div>
      <div class="author">Krishna Prasad S</div>
    </div>
  </div>
</body>
</html>

```

### styles.css
```css
.cover{
  width: 360px;
  height: 540px;
  margin: 40px auto;
  border-radius: 12px;
  box-shadow: 0 12px 30px rgba(0,0,0,0.25);
  background: linear-gradient(180deg, #1b2735 0%, #0f1622 100%);
  color: #b5b5b5;
  position: relative;
  overflow: hidden;
  font-family: 'Georgia', serif;
}

.cover-inner{
  padding: 36px 28px;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  position: relative;
}

.cover::before{
  content: '';
  position: absolute;
  left: -80px;
  bottom: -60px;
  width: 520px;
  height: 300px;
  background: radial-gradient(circle at 30% 20%, rgba(255,255,255,0.06), transparent 25%),
              radial-gradient(circle at 70% 60%, rgba(255,255,255,0.03), transparent 25%);
  transform: rotate(-10deg);
  opacity: 0.9;
}

/* Title */
.title{
  font-size: 36px;
  line-height: 1.02;
  margin: 0 0 10px 0;
  letter-spacing: 0.6px;
  color: #ffefc4;
  text-shadow: 0 3px 12px rgba(0,0,0,0.6);
}

/* Subtitle */
.subtitle{
  font-size: 16px;
  margin: 0 0 16px 0;
  color: #dfe7ea;
  font-style: italic;
}

/* Tagline */
.tag{
  font-size: 14px;
  color: #c8d2d6;
  max-width: 260px;
}

/* Author */
.author{
  position: absolute;
  right: 18px;
  bottom: 18px;
  font-size: 13px;
  color: #bcd0d6;
  transform: rotate(-90deg);
  transform-origin: right bottom;
  letter-spacing: 1px;
}

.spine{
  position: absolute;
  left: -40px;
  top: 50%;
  transform: rotate(-90deg) translateY(-50%);
  color: rgba(255,255,255,0.08);
  font-size: 12px;
  letter-spacing: 2px;
}

@media (max-width:480px){
  .cover{transform: scale(0.9); margin:20px auto;}
  .title{font-size:28px;}
}

```

## OUTPUT:
<img width="1919" height="967" alt="Screenshot 2025-11-25 185615" src="https://github.com/user-attachments/assets/57342526-0705-407a-931e-6bab9dce1342" />


## RESULT:

Thus, The book cover was successfully designed using HTML and CSS and displays correctly in the browser.

