Project 1: E-Commerce Inventory Dashboard (Build New - Data-Driven Semantic Layout)
Objective: Develop a single-page e-commerce dashboard titled "TechGear Inventory Hub" that visualizes and manages a product catalog inspired by your uploaded inventory screenshot. This project integrates all HTML topics from Day-001 (fundamentals, semantics) and Day-002 (lists, tables, forms)—from basic structure to exhaustive form interactions—into a cohesive admin panel. The challenge: Recreate the screenshot's messy table with semantic fixes (e.g., proper thead/tbody), embed grocery-style lists for categorization, and build a multi-input form for stock updates, ensuring 100% validation and ARIA compliance. Hard due to data accuracy (fix duplicates like the two "Wireless Mouse" entries) and nesting (tables in articles), but achievable by templating from your handwritten notes' tag snippets.

Requirements (Exhaustive Coverage – Zero Skips):

DOCTYPE, Basic Structure (html, head, body): <!DOCTYPE html>. <head>: <title>TechGear Inventory Hub</title>, <meta charset="UTF-8">, <meta name="viewport" content="width=device-width, initial-scale=1">, <meta name="description" content="Day 1-2 HTML: Product Inventory Dashboard">, <meta name="keywords" content="inventory, table, form, semantics">. <body> wraps all.
Headings & Text Content (h1-h6, p, strong, em): Hierarchy: <h1> dashboard title in header. <h2> for sections (e.g., "Product Catalog"), <h3> for categories, <h4-h6> for item details (e.g., <h6>Stock Alert</h6>). 3-5 paragraphs per section with <strong> (e.g., "Low stock items") and <em> (e.g., "urgent restock").
Block vs. Inline Elements (div, span): <div> only for non-semantic wrappers like a dashboard grid (<div class="grid">). <span> inline for 4 highlights (e.g., <span class="price-tag">$25.99</span> in table cells).
Links & Navigation (a, nav): <nav> with <ul> of 5 anchors: Dashboard, Catalog, Add Product, Reports, Export (e.g., <a href="#catalog">View Inventory</a>). External: <a href="export.csv" download title="Download CSV">Export Data</a>.
Images & Media (img, figure/figcaption): 4 placeholders: <img src="mouse.jpg" alt="Wireless Mouse Preview" width="100" height="100" loading="lazy"> in catalog. Wrap 2 in <figure><figcaption>Ergonomic Design - From Inventory Notes</figcaption></figure>.
Lists (ul, ol, dl): Category <ul> for products (5 bullets: Mice, Keyboards, etc.). <ol> for restock steps (4 numbered: 1. Check low stock, ...). <dl> for specs (e.g., <dt>ID</dt><dd>101</dd> – 3 pairs per item).
Tables (table, thead, tbody, tfoot, th, td): Core: Fixed inventory table from screenshot (4 rows + total; fix duplicates by merging Wireless Mouse entries). <thead>: <th scope="col">ID</th>, etc. <tbody>: Data with rowspan for merged rows. <tfoot>: Totals row (e.g., <td colspan="3">4 Products</td><td>$665.56 Total Value</td>). Add headers="id-col" for accessibility.
Semantic Elements (header, nav, main, section, article, aside, footer): <header>: h1 + nav. <main>: Journey core. 4 <article>s in <section id="catalog"> (each product: h3, table snippet, lists). <aside>: dl alerts + ul quick actions. <footer>: p summary, ul links.
Forms & Inputs (form, input types, label, select, textarea, button): "Add/Update Product" form (<form action="/update" method="post">):
Text: <label for="name">Product Name</label><input type="text" id="name" required pattern="[A-Za-z\s]+" title="Letters only">.
Number: <input type="number" min="1" max="999" step="1" value="101"> for ID.
Email: <input type="email" placeholder="supplier@email.com"> for vendor.
Tel: <input type="tel" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}"> for support.
Date: <input type="date" min="2025-12-01"> for restock date.
Time: <input type="time"> for shift availability.
Range: <label for="stock-level">Stock Slider</label><input type="range" id="stock-level" min="0" max="300"><output for="stock-level"></output>.
Month/Week: <input type="month"> for quarterly review, <input type="week"> for weekly audit.
Color: <input type="color" value="#000000"> for product theme.
Checkbox: <fieldset><legend>Categories</legend><input type="checkbox" name="cat" value="peripheral" checked> Peripheral</fieldset> (4 options).
Radio: <input type="radio" name="status" value="active"> Active (3: Active, Low, Out).
Select: <label for="type">Type</label><select id="type" required><optgroup label="Accessories"><option>Mouse</option></optgroup></select> (5 opts).
Textarea: <label for="desc">Description</label><textarea id="desc" rows="4" cols="40" maxlength="200" placeholder="e.g., Ergonomic with USB"></textarea>.
File: <input type="file" accept="image/*,.pdf" multiple> for photos/specs.
Hidden: <input type="hidden" name="total-products" value="4">.
Buttons: <button type="submit">Update Inventory</button>, <button type="reset">Clear</button>.
3 fieldsets; <datalist id="desc-suggestions"><option>RGB lighting</option></datalist> for textarea.
Accessibility & SEO: <html lang="en">. aria-label="Product Navigation" on nav, role="grid" on table. Alt/title everywhere, tabindex="0" on sections. SEO: <link rel="canonical" href="/">, OG metas (e.g., <meta property="og:title" content="TechGear Inventory">).
Files Integration: Use inventory screenshot data exactly (fix table errors like missing descriptions). Embed grocery ul/ol/dl as "Supply Chain List" in aside (e.g., ul fruits as peripherals). Handwritten notes: <details><summary>Day 1-2 Notes</summary><pre><code>&lt;table&gt;...&lt;/table&gt;</code></pre></details> with tag snippet.
Challenge Level: Hard—calculate tfoot totals manually from data (e.g., sum prices/stocks), nest form outputs in preview dl (e.g., "New Stock: 150"), validate screenshot fidelity. Time: 4-6 hours. Test: Browser + NVDA for form/table flow. Output: index.html, commit "Day-1-2-Inventory-Build".

Why Best: Mirrors real admin panels (e.g., Shopify dashboard), forcing error-prone data cleanup and semantic tables—builds pro-level precision from your files.
