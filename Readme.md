# **Tailwind Fundamentals & Configure Tailwind CSS**
## 1. **Install Tailwind CSS in a project & configure**
Tailwind CSS is already installed in Next.js. When we use Tailwind CSS in another framework, we have to install it separately.
## 2. **Understand utility-first CSS** ##
Utility-first CSS is a CSS approach where small, single-purpose utility classes are combined directly in HTML to create the desired design.<br>
### For example
```
<button class="bg-blue-500 text-white px-4 py-2 rounded">
   Click Me
</button>
```
In Tailwind CSS, we can use short utility classes. For example, we use `bg` instead of writing the complete CSS property `background-color`. In traditional CSS, we normally have to write the complete property name, such as `background-color`.
## 3. **Apply text colors**
In Tailwind CSS, we use this class to change the text color.
### **For example**
```
<p className="text-blue-100">
  Text color change property
</p>
```
## 4. **Apply background color**
In Tailwind CSS, we use this class to change the background color.
### **For example**
```
<p className="bg-black-300">
  Background color change property
</p>
```
## 5. **Apply border color**
In Tailwind CSS, we use this class to change the border color.
### **For example**
```
<p className="border-blue-100">
  Border color change property
</p>
```
## 6. **Set font size**
In Tailwind CSS,we use this class to set font size.
### **For example**
```
<p className="text-xl">
  Font size change property
</p>
```
```
text-sm → small
text-base → normal
text-lg → large
text-xl → extra large
text-2xl → more large
text-4xl → very large
```
## 7. **Set font weight**
In Tailwind CSS,we use this class to set font weight.
### **For example**
```
<p class="text-4xl font-bold">
  Welcome
</p>
```
```
font-thin → bahut thin
font-light → halka
font-normal → normal
font-medium → medium
font-semibold → semi-bold
font-bold → bold
font-extrabold → extra bold
font-black → sab se zyada bold
```
## 8. **Set line height**
In Tailwind CSS,we use this class to set line height.
### **For example**
```
<p class="leading-8">
  This is a paragraph with increased line height & space.
</p>
```
```
leading-none → no extra line height
leading-tight → tight
leading-normal → normal
leading-relaxed → more space
leading-loose → much more space
```
## 9. **Set letter spacing**
In Tailwind CSS, you can set letter spacing using `tracking-*` classes.
### **For example**
```
<h1 className="text-4xl font-bold tracking-widest">
  Hello World
</h1>
```
tracking-widest → tracking-wide → tracking-tight
## 10. **Set element widght**
In Tailwind CSS, you can set element widght using `w-*` classes.
### **For example**
```
<h1 className="w-96">
  Hello World
</h1>
```
## 11. **Set element height**
In Tailwind CSS, you can set element height using `h-*` classes.
### **For example**
```
<h1 className="h-96">
  Hello World
</h1>
```
## 12. **Set minimum/maximum width**
Set minimum/maximum width in Tailwind CSS using min-w-* and max-w-* classes.
1. min-w-* → Sets the minimum width
2. max-w-* → Sets the maximum width
### **For example**
```
<div class="min-w-[300px] max-w-[500px]">
  Content
</div>
```
```
<div class="max-w-sm">Content</div>
<div class="max-w-md">Content</div>
<div class="max-w-lg">Content</div>
<div class="max-w-full">Content</div>
```
## 13. **Set minimum/maximum height**
Tailwind CSS mein minimum/maximum height set karne ke liye min-h-* aur max-h-* classes use hoti hain.
* `min-h-*` → Minimum height
* `max-h-*` → Maximum height
### **For example**
```
<div class="min-h-[200px] max-h-[500px]">
  Content
</div>
```
## 14. **Apply padding**
In Tailwind CSS, `p-*` classes are used to apply padding.

* `p-*` → Padding on all sides
* `px-*` → Left and right padding
* `py-*` → Top and bottom padding
* `pt-*` → Top padding
* `pb-*` → Bottom padding
* `ps-*` → Start padding
* `pe-*` → End padding
### **For example**
```
<div class="p-[20px]">
  Content
</div>
```
## 15. **Apply margin**
Apply margin in Tailwind CSS using m-* classes.
* `m-*` → All sides margin
* `mx-*` → Left + right margin
* `my-*` → Top + bottom margin
* `mt-*` → Top margin
* `mb-*` → Bottom margin
* `ms-*` → Start margin
* `me-*` → End margin
### **For example**
```
<div class="m-4">
  Content
</div>
```
## 16. **Understand Spacing Scale**
In Tailwind CSS, the **spacing scale** means predefined spacing values that are used for **margin, padding, gap, width, height**, etc.
### **For example**
```
<div class="p-4">
   Content
</div>
```
Here, `4` in `p-4` represents a value from the spacing scale.
Common spacing values:
| Class  | Default size |
| ------ | -----------: |
| `p-1`  |          4px |
| `p-2`  |          8px |
| `p-3`  |         12px |
| `p-4`  |         16px |
| `p-5`  |         20px |
| `p-6`  |         24px |
| `p-8`  |         32px |
| `p-10` |         40px |
| `p-12` |         48px |
**Simple rule:**
`1 spacing unit = 4px`
So:
`p-4 = 4 × 4px = 16px`
The same spacing scale is used with `m-*`, `gap-*`, `w-*`, `h-*`, and other spacing utilities.
## 17. **Use Arbitrary Values**
In Tailwind CSS, arbitrary values allow you to use custom values that are not available in the default spacing scale.
### **For example**
```
<div class="w-[420px]">
  Content
</div>
```
**Here, w-[420px] sets the element's width to exactly 420px.**
Other examples:
```
<div class="p-[25px]">Content</div>
<div class="mt-[35px]">Content</div>
<div class="h-[300px]">Content</div>
```
Simple rule:
Use square brackets [ ] when you want to provide a custom value.

`w-[420px] → Width = 420px.`
## 18. **Combine Multiple Utilities Correctly**
Tailwind CSS mein aap multiple utility classes ko ek hi element par combine kar sakte hain.
### **For example**
```
<div class="w-[420px] p-4 mt-6 bg-blue-500 text-white rounded-lg">
  Content
</div>
```
**This**:
* `w-[420px]` → Width = 420px
* `p-4` → Padding
* `mt-6` → Top margin
* `bg-blue-500` → Background color
* `text-white` → Text color
* `rounded-lg` → Rounded corners
### Simple rule:
Multiple Tailwind utilities ko space ke saath ek hi class attribute mein likha jata hai.
