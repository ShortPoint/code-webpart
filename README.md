# 🧩 SharePoint Code Editor WebPart
Welcome to the SharePoint Code Editor WebPart – a powerful, flexible, and community-first solution that empowers you to write and embed custom code (HTML, CSS, and JavaScript) directly into SharePoint pages. Designed with safety, usability, and collaboration in mind, this web part is completely free and open to the SharePoint community.

## ✨ Features

### 🧪 Sandbox Mode
Run your code safely in an isolated `<iframe>` environment. This prevents broken or untrusted code from affecting the rest of your SharePoint page.

### 👁️ Visibility Control
Target specific devices where you want your webpart to appear, wether its for Desktop, Tablet or Mobile Devices.

### 🛠️ Built-in Testing Tools
If something goes wrong, no need to panic. Simply add `?spdisablecode=1` (or `&spdisablecode=1` if the URL has other parameters) to your URL to instantly disable the web part and regain control.

### 🔖 Smart Tags (Dynamic Variables)
Our favorite feature! Define variables inside your code using special tags, and they’ll appear as editable fields in the UI. This allows non-technical users to easily update code behavior without touching the code, making it portable, reusable, and shareable, here's how you can use it:

🧠 Syntax
```
/* FieldN ||| LABEL ||| DEFAULT_VALUE */
```

* `FieldN` — a unique field key where `N` ranges from `0` to `19` (up to 20 custom fields per web part).
* `LABEL` — the name shown next to the input field in the UI.

* `DEFAULT_VALUE` — (optional) a fallback value that will be used if no input is provided.

**Examples**

in HTML
```
<h1>/* Field0 ||| Title ||| Welcome to our Portal */</h1>
```

in JavaScript
```
const color = '/* Field1 ||| Text Color ||| #333 */';
```

in CSS
```
.example-element {
    font-family: sans-serif;
    font-size: /* Field2 ||| CSS Field ||| 30px */;
    text-align: center;
}
```

Here's a quick live demonstration on how to embed a configurable stock widget into a SharePoint Page, you can find the [source also here](/ShortPoint/code-webpart/blob/main/samples/stock-widget.html)

![Demo of Code Web Part](https://p69.f3.n0.cdn.zight.com/items/bLu2x7vp/a8da9219-0019-49a3-b245-515cfa252de2.gif?source=viewer&v=694a927cf4701cc575075416eefe1cc0)

### ⬇️ Import & Export
Easily export your code (HTML, CSS, JS) from one instance and import it into another with a single click. Perfect for replicating setups across multiple pages or sites.

## 📥 Download

👉 Download the latest [Code WebPart](https://www.shortpoint.com/code-webpart)

Deploy it to your SharePoint site and start customizing your pages in minutes.

## 💡 Code Samples
Looking for inspiration or ready-to-use snippets?

📂 Check out our [Code Samples Directory](/ShortPoint/code-webpart/tree/main/samples) — a growing collection of free, copy-paste-ready examples covering various use cases, from banners to calculators and more.

## 💬 Ideas & Feedback
Have an idea to improve the web part? Found a bug? Want to share how you're using it?

We'd love to hear from you! Join the conversation in our [GitHub Discussions Page](/ShortPoint/code-webpart/discussions/) — it's the best place to:

 * [Ask questions you’re wondering about](/ShortPoint/code-webpart/discussions/categories/q-a) and Engage with other community members.
  * [Share ideas](/ShortPoint/code-webpart/discussions/categories/ideas): Share ideas for new features, and we will build it
  * [Show and tell](/ShortPoint/code-webpart/discussions/categories/show-and-tell): built something useful using the code webpart, showcase your work here!

Your input helps shape the future of this tool for the entire SharePoint community.


🧡 A Gift to the Community
This project is built and maintained with love for the SharePoint team. We hope it empowers you to do more with less.
