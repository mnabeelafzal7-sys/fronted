# **Tailwind Fundamentals & Configure Tailwind CSS**
## 1. **Install Tailwind CSS in a project & configure**
Tailwind CSS is already installed in Next.js. When we use Tailwind CSS in another project, we have to install it separately.
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
```
<p className="text-blue-100">
  Text color change property
</p>
```
## 4. **Apply background color**
In Tailwind CSS, we use this class to change the background color.
```
<p className="bg-black-300">
  Background color change property
</p>
```
## 5. **Apply border color**
In Tailwind CSS, we use this class to change the border color.
```
<p className="border-blue-100">
  Border color change property
</p>
```
## 6. **Set font size**
In Tailwind CSS,we use this class to set font size.
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
