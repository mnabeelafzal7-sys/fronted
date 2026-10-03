# **Layout Mastery**
## 1. **Understand CSS box model through Tailwind**
The CSS **Box Model** means that every **HTML element** is considered a box.**This box has 4 main parts:**<br>
### **Content → Padding → Border → Margin**<br>
In Tailwind CSS, we control these using **utility classes.**
```
<div class="w-64 p-4 border-2 m-4">
  Content
</div>
```
* `w-64` → **Content/element width**
* `p-4` → **Padding** — content aur border ke darmiyan space
* `border-2` → **Border** — element ke around line
* `m-4` → **Margin** — element ke bahar space<br>
**In tailwind**
`w/h` → size
`p-*` → padding
`border-*` → border
`m-*` → margin
## 2. **Use block**
Tailwind CSS mein `block` utility element ko **block-level element** banati hai.
```
<div class="block">
  Hello World
</div>
```
Use this class in side **element blocks**.
```
<span class="block bg-blue-500 p-4">
  Hello World
</span>
```
**Yahan:**
* `block` → element ko new line par rakhta hai
* `bg-blue-500` → background color
* `p-4` → padding
Simple: block → element ko block-level banata hai.

## 3. **Use inline**
Tailwind CSS's inline utility makes an element an inline-level element.
```
<div>
  <span class="inline bg-blue-500">
    Hello
  </span>
  <span class="inline bg-red-500">
    World
  </span>
</div>
```
**Here:**
* `inline* → keeps the element on **the same line**.<br>
* It normally takes only the **width required by its content**.<br>
* The next inline element can **appear on the same line**.<br>
**Simple rule:**<br>
* `inline` → makes an element **inline-level and helps keep elements** on the same line.
## 4. **Use inline-block**
Tailwind CSS's `inline-block` utility makes an element an **inline-block element**.
```
<span class="inline-block bg-blue-500 p-4">
  Hello
</span>
<span class="inline-block bg-red-500 p-4">
  World
</span>
```
**Here**:<br>
inline-block → elements can stay on **the same line**.<br>
* `p-4` → **applies padding**.<br>
* `bg-blue-500` → gives the element a **background color**.<br>
The advantage of `inline-block` is that the element stays on the **same line like inline**, but you can properly **control its width, height, padding, and margin**.<br>
Simple rule:<br>
* `inline` → same line **+ limited box control**<br>
* `inline-block` → same line **+ width/height/padding/margin** control
## 5. **Use flex**
Tailwind CSS's flex utility makes an element a **flex container**. It allows you to **easily arrange and align its child elements**.
```
<div class="flex">
  <p>One</p>
  <p>Two</p>
  <p>Three</p>
</div>
```
By default, the items appear in a **row (horizontal) direction**.
Example with gap
```
<div class="flex gap-4">
  <p class="bg-blue-500 p-4">One</p>
  <p class="bg-red-500 p-4">Two</p>
  <p class="bg-green-500 p-4">Three</p>
</div>
```
**Here:**<br>
* `flex` → enables the **Flexbox layout**.<br>
* `gap-4` → **adds space** between the items.<br>
* `p-4` → **adds padding inside** each item.<br>
**Simple rule:**<br>
* `flex` → used to arrange child elements in a flexible layout.
## 6. **Use flex-row**
Tailwind CSS's **flex-row utility arranges flex items in a horizontal direction**.
```
<div class="flex flex-row">
  <p>One</p>
  <p>Two</p>
  <p>Three</p>
</div>
```
**Output:**
```
One   Two   Three
```
**Here:**<br>
* `flex` → **enables the Flexbox layout**.<br>
flex-row → arranges items from **left to right (horizontal)**.<br>
**Simple rule**:<br>
*`flex-row` → Flex items are **arranged in a row (horizontal)**.
## 7. **Use flex-col**
Tailwind CSS's **flex-col utility** arranges flex items in a **vertical direction**.
```
<div class="flex flex-col">
  <p>One</p>
  <p>Two</p>
  <p>Three</p>
</div>
```
**Output:**
```
One
Two
Three
```
**Here:**<br>
* `flex` → enables **the Flexbox layout**.<br>
* `flex-col` → arranges items from **top to bottom (vertical)**.<br>
**Simple rule:**<br>
* `flex-col` → Flex items are **arranged in a column (vertical)**.
## 8. **Use flex-wrap**
Tailwind CSS's flex-wrap utility is used to move flex items to the next line (wrap) when there is not enough space in the container.
```
<div class="flex flex-wrap gap-4">
  <p class="w-40 bg-blue-500 p-4">One</p>
  <p class="w-40 bg-red-500 p-4">Two</p>
  <p class="w-40 bg-green-500 p-4">Three</p>
  <p class="w-40 bg-yellow-500 p-4">Four</p>
</div>
```
**Here:**<br>
* `flex` → **enables Flexbox**.<br>
* `flex-wrap` → allows items to **wrap to the next line**.<br>
* `gap-4` → **adds space between** the items.<br>
* `w-40` → **sets the width** of each item.<br>
Simple rule:<br>
* `flex-wrap` → When there isn't enough space in one row, items move to the next line.
## 9. **Use justify-**
Tailwind CSS mein **justify-* utilities** ka use **flex ya grid items ko main axis par align karne** ke liye hota hai.
**Example**
```
<div class="flex justify-center">
  <div>One</div>
  <div>Two</div>
  <div>Three</div>
</div>
```
**Common classes**<br>
*`justify-start` → Items ko **start mein rakhta hai**.<br>
*`justify-center` → Items ko **center mein rakhta hai**.<br>
*`justify-end` → Items ko **end mein rakhta hai**.<br>
*`justify-between` → Items ke **darmiyan equal space deta hai**.<br>
*`justify-around` → Items ke **around space deta hai**.<br>
*`justify-evenly` → Items ke **darmiyan equal space deta hai**.<br>
**Example with justify-between**
```
<div class="flex justify-between">
  <p>Logo</p>
  <p>Menu</p>
</div>
```
**Simple rule**:<br>
*`justify-*` → Items ko** main axis par position/align karne ke** liye use hota hai.<br>
Important: Agar **flex-row hai**, to main **axis horizontal hoti hai**. Agar **flex-col** hai, to** main axis vertical** hoti hai.
## 10. **Use items-**
Tailwind CSS mein **`items-*` utilities** ka use flex ya grid items ko **cross axis par align** karne ke liye hota hai.
**Example:**
```
<div class="flex items-center h-40">
  <div class="bg-blue-500 p-4">One</div>
  <div class="bg-red-500 p-4">Two</div>
  <div class="bg-green-500 p-4">Three</div>
</div>
```
**Common classes**:<br>
* `items-start` → Items ko **start par align** karta hai.<br>
* `items-center` → Items ko **center mein align** karta hai.<br>
* `items-end` → Items ko **end par align** karta hai.<br>
* `items-baseline` → Items ko **text baseline par align** karta hai.<br>
* `items-stretch` → Items ko available **cross-axis space** mein stretch karta hai.<br>
**Example**
```
<div class="flex items-center h-40">
  <p>Logo</p>
  <p>Menu</p>
</div>
```
**Yahan**:<br>
flex` → Flexbox **layout enable** karta hai.<br>
items-center` → Items ko **vertically center karta** hai (row direction mein).<br>
**Simple rule**:<br>
* `items-*` → Items ko **cross axis par align karne** ke liye use hota hai.<br>
**Difference**:<br>
* `justify-*` → **Main axis**<br>
* `items-*` → **Cross axis**
## 11. **Use content-**
In Tailwind CSS, `content-*` utilities are used with **Flexbox and Grid to align the entire group** of items along the **cross axis** when there is extra space in the container.<br>
They work when the container has multiple **rows or columns**, usually with **flex-wrap or a grid layout**.<br>
**Example**
```
<div class="flex flex-wrap content-center h-64 gap-4">
  <p class="bg-blue-500 p-4">One</p>
  <p class="bg-blue-500 p-4">Two</p>
  <p class="bg-blue-500 p-4">Three</p>
  <p class="bg-blue-500 p-4">Four</p>
</div>
```
**Common classes**<br>
* `content-start` → **Aligns rows at the start**.<br>
* `content-center` → Aligns the **group of rows in the center**.<br>
* `content-end` → Aligns **rows at the end**.<br>
* `content-between` → Adds **equal space between rows**.<br>
* `content-around` → Adds **space around rows**.<br>
* `content-evenly` → Adds **equal space around and between rows**.<br>
* `content-stretch` → **Stretches rows to fill the available space.**<br>
**Simple rule**<br>
items-* aligns **individual items within a row**.<br>
* `content-*` aligns the **group of rows inside the container**.<br>
**Note:** `content-*` is most noticeable when the container has extra height and its items wrap into multiple rows.
## 12. **Use gap-**
In Tailwind CSS, gap-* utilities add space between items in a Flexbox or Grid container.<br>
**Example**
```
<div class="flex gap-4">
  <p class="bg-blue-500 p-4">One</p>
  <p class="bg-red-500 p-4">Two</p>
  <p class="bg-green-500 p-4">Three</p>
</div>
```
**Here**, gap-4 adds 16px of space between the items.<br>
Common classes<br>
* `gap-2` → **8px space** between items<br>
* `gap-4` → **16px space** between items<br>
* `gap-6` → **24px space** between items<br>
* `gap-8` → **32px space** between items<br>
* `gap-x-4` → **Horizontal gap** of 16px<br>
* `gap-y-4` → **Vertical gap** of 16px<br>
**Simple rule**<br>
* `gap-*` adds space in **both directions**.<br>
* `gap-x-*` adds **horizontal space**.<br>
* `gap-y-*` adds **vertical space**.<br>
Note: `gap-*` creates space between items, not around the **outside of the container**.
## 13. **Use space-x-**
In Tailwind CSS, space-x-* utilities add **horizontal space between child elements**.<br>
**Example**
```
<div class="flex space-x-4">
  <p class="bg-blue-500 p-4">One</p>
  <p class="bg-red-500 p-4">Two</p>
  <p class="bg-green-500 p-4">Three</p>
</div>
```
**Here**, space-x-4 adds 16px of **horizontal space** between the child elements.<br>
**Common classes**<br>
* `space-x-2` → **8px horizontal** space<br>
* `space-x-4` → **16px horizontal** space<br>
* `space-x-6` → **24px horizontal** space<br>
* `space-x-8` → **32px horizontal** space<br>
**Simple rule**<br>
* `space-x-*` → Adds space between **items horizontally**.<br>
* `space-y-*` → Adds space between **items vertically**.
## 14. **Use grid**
In Tailwind CSS, the **grid utility makes an element a CSS Grid container**. It allows you to **arrange child elements in rows and columns**.<br>
Example
```
<div class="grid grid-cols-3 gap-4">
  <p class="bg-blue-500 p-4">One</p>
  <p class="bg-red-500 p-4">Two</p>
  <p class="bg-green-500 p-4">Three</p>
  <p class="bg-yellow-500 p-4">Four</p>
  <p class="bg-purple-500 p-4">Five</p>
  <p class="bg-pink-500 p-4">Six</p>
</div>
```
**Here**:<br>
* `grid` → **Enables CSS Grid**.<br>
* `grid-cols-3` → Creates **3 equal-width columns**.<br>
* `gap-4` → Adds 16px space **between rows and columns**.<br>
* `p-4` → Adds 16px **padding inside each item**.<br>
**Common classes**<br>
* `grid-cols-2` → **2 columns**<br>
* `grid-cols-3` → **3 columns**<br>
* `grid-cols-4` → **4 columns**<br>
* `grid-rows-2` → **2 rows**<br>
gap-4 → **Space between items**<br>
**Simple rule**<br>
Use grid when you want to arrange items in **both rows and columns**, such as image **galleries, product cards, or dashboards**.<br>
**Remember**: grid only enables the grid layout. Use `grid-cols-*` to define how many columns you want.
## 15. **Define Grid Columns**
In Tailwind CSS, `grid-cols-*` utilities define how many **columns a Grid container has and how** the available space is divided between them.<br>
**Example**
```
<div class="grid grid-cols-3 gap-4">
  <p class="bg-blue-500 p-4">One</p>
  <p class="bg-red-500 p-4">Two</p>
  <p class="bg-green-500 p-4">Three</p>
  <p class="bg-yellow-500 p-4">Four</p>
  <p class="bg-purple-500 p-4">Five</p>
  <p class="bg-pink-500 p-4">Six</p>
</div>
```
**Here**, `grid-cols-3` creates **3 equal-width columns**. The six items are arranged in **2 rows, with 3 items in each row**.<br>
**Common classes**<br>
* `grid-cols-1` → **1 column**<br>
* `grid-cols-2` → **2 equal-width** columns<br>
* `grid-cols-3`→ **3 equal-width** columns<br>
* `grid-cols-4`→ **4 equal-width** columns<br>
* `grid-cols-6` → **6 equal-width** columns<br>
**Simple rule**<br>
`grid-cols-3` means **divide the grid** into 3 equal columns.<br>
**Remember:** grid enables the grid layout, while `grid-cols-*` defines **the number of columns**.
## 16. **Define Grid Rows**
In Tailwind CSS, `grid-rows-*` utilities define how many rows a **Grid container has and how** the available space is divided between them.<br>
**Example**
```
<div class="grid grid-rows-2 grid-flow-col gap-4 h-64">
  <p class="bg-blue-500 p-4">One</p>
  <p class="bg-red-500 p-4">Two</p>
  <p class="bg-green-500 p-4">Three</p>
  <p class="bg-yellow-500 p-4">Four</p>
</div>
```
Here:<br>
* `grid` → **Enables CSS Grid**.<br>
* `grid-rows-2` → Creates **2 equal-height rows**.<br>
* `grid-flow-col` → Places items down the rows first, then **starts a new column**.<br>
* `h-64` → Gives the grid a **height of 256px**.<br>
* `gap-4` → Adds **16px space between items**.<br>
Common classes<br>
* `grid-rows-1` → 1 row<br>
* `grid-rows-2` → 2 equal-height rows<br>
* `grid-rows-3` → 3 equal-height rows<br>
* `grid-rows-4` → 4 equal-height rows<br>
Simple rule<br>
`grid-rows-2` means divide the grid into 2 rows.<br>
**Remember:** grid-cols-* defines columns, while `grid-rows-*` defines rows. `grid-rows-*` sets the row sizes; it does not by itself control the order in which items fill the grid.
## 17. **Use col-span-**
In Tailwind CSS, `col-span-*` utilities control how many columns a **grid item occupies**.<br>
Example
```
<div class="grid grid-cols-3 gap-4">
  <p class="col-span-2 bg-blue-500 p-4">One</p>
  <p class="bg-red-500 p-4">Two</p>
  <p class="bg-green-500 p-4">Three</p>
  <p class="bg-yellow-500 p-4">Four</p>
</div>
```
**Here**:<br>
* `grid-cols-3` → **Creates 3 columns**.<br>
* `col-span-2` → Makes the **first item occupy 2 columns**.<br>
* The other items occupy **1 column each**.<br>
Common classes<br>
* `col-span-1` → Occupies 1 column.<br>
* `col-span-2` → Occupies 2 columns.<br>
* `col-span-3` → Occupies 3 columns.<br>
* `col-span-full` → Occupies all columns.<br>
**Simple rule**<br>
`col-span-2` means make this grid item take the space of 2 columns.<br>
Remember: `grid-cols-*` defines the grid columns, while `col-span-*` defines how many of those **columns an individual item occupies**.
## 18. **Use responsive grids**
In Tailwind CSS, responsive grid utilities allow you to change the number of columns based on the screen size.<br>
This helps your layout look good on **mobile, tablet, and desktop screens**.<br>
**Example**
```
<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4">
  <p class="bg-blue-500 p-4">One</p>
  <p class="bg-red-500 p-4">Two</p>
  <p class="bg-green-500 p-4">Three</p>
  <p class="bg-yellow-500 p-4">Four</p>
  <p class="bg-purple-500 p-4">Five</p>
  <p class="bg-pink-500 p-4">Six</p>
</div>
```
Explanation<br>
* `grid` → Enables CSS Grid.<br>
* `grid-cols-1` → Shows 1 column by default (mobile).<br>
* `sm:grid-cols-2` → Shows 2 columns on small screens and larger.<br>
* `lg:grid-cols-3` → Shows 3 columns on large screens and larger.<br>
* `gap-4` → Adds 16px space between items.<br>
Responsive breakpoints<br>
| Prefix |  Minimum screen width |
| ------ |   --------: |
| `sm:`  | 768px        |
| `md:`  |        640px |
| `lg:`  |       1024px |
| `xl:`  |       1280px |
| `2xl:` |       1536px |

**Simple rule**<br>
`sm:grid-cols-2` means use 2 columns when the screen reaches the **sm breakpoint or wider**.<br>
**Remember:** Tailwind uses a mobile-first approach. The class without a prefix **applies by default, and prefixed classes apply at that breakpoint and larger**.
