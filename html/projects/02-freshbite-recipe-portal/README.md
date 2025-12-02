Project 2: Recipe & Feedback Portal (Enhance Existing - Form-Centric Integration)
Objective: Transform a basic "Contact Us" page (assume simple form from Day-001 notes) into "FreshBite Recipe Portal," a user-submission site blending grocery lists with inventory feedback forms. Layer all Day-001/002 topics for a submission/review flow: Grocery ol as recipe steps, inventory table for ingredient stocks, advanced forms for recipes. Difficulty: Enhance without breaking original (wrap form in main), integrate screenshot data as stock checker, add 20+ inputs with patterns—hard nesting (forms in sections), but use handwritten snippets for quick wins.

Requirements (Full Integration – No Skips, Enhances Simple Base):

DOCTYPE, Basic Structure: Reuse simple's doctype/head (add <meta name="robots" content="index">, keywords: "recipe, form, list"). Body: Add main around original form.
Headings & Text Content: Original h1 ("Contact") to h2. New <h1>: "FreshBite Recipes". <h3-h6> for 6 recipes (e.g., <h4>Ingredient List</h4><h6>From Grocery Notes</h6>), ps with strong/em (e.g., "Fresh ingredients only! Per your notes.").
Block vs. Inline: Replace simple divs with semantics. <span class="alert">Low Stock</span> inline in table (3 uses).
Links & Navigation: Enhance simple links: <nav><ul> "Home | Recipes | Submit | Stock Check" (anchor #submit). External: <a href="grocery.pdf" download>Download List</a>.
Images & Media: Original img? Add figcaption: "Recipe Hero - Day 2". New: 3 grocery imgs (e.g., <img src="apples.jpg" alt="Fresh Apples" width="150"> in ul), footer cert img.
Lists (ul, ol, dl): Original ul? Nest in aside. Recipes: <ul> ingredients from grocery (nested sub-ul: Fruits > Apples/Bananas). <ol> prep steps (4 numbered, exact from file). <dl> nutrition (e.g., <dt>Calories</dt><dd>200</dd> – 4 pairs).
Tables: New stock table from inventory screenshot in section (thead: ID | Name | Price | Stock; tbody: 4 rows, fix Wireless Mouse dup; tfoot: Averages). Scope on th; enhances simple's potential data.
Semantic Elements: Original form in <aside>. <header>: h1 + nav. <main><section id="recipes"><article> per recipe (2 articles: h3, lists/table). <footer>: Table summary + original ul.
Forms & Inputs: Enhanced submission form (<form id="recipe-form">, 4 fieldsets):
Text: <input type="text" required placeholder="Recipe Name"> (pattern for title case).
Search: <input type="search" list="ing-suggest"> for ingredients.
Url: <input type="url"> for source link.
Number/Range: <input type="number" min="1" max="10" step="0.5"> servings; range for spice level.
Date/Month: <input type="date"> expiry, <input type="month"> seasonal.
Time/Week: <input type="time"> prep time, <input type="week"> meal plan.
Color: <input type="color"> for plating theme.
Checkbox/Radio: Checkboxes for dietary (Vegan, etc., 5); radios for difficulty (Easy/Hard, 3).
Select: <select><optgroup label="Grocery"><option>Apples</option></optgroup></select> (6 opts from file).
Textarea: <textarea placeholder="Full Steps" rows="8" maxlength="500"></textarea>.
File: <input type="file" accept="image/*"> for photo.
Hidden: <input type="hidden" name="day" value="1-2">. Buttons: <button type="submit">Submit Recipe</button>, "Preview" (type=button). Outputs: <output id="servings"></output>. Datalist from grocery ul.
Accessibility & SEO: aria-labelledby on sections, role="form" on submit. aria-invalid on patterns. SEO: Breadcrumb ol, schema <script type="application/ld+json">{"@type":"Recipe","name":"Salad"}</script>.
Files Integration: Grocery ul/ol/dl as recipe base (e.g., ul fruits in form select). Inventory table for "Stock Check" section (query via form range). Handwritten: <iframe src="notes.html" title="Day Notes" width="100%" height="300"></iframe> (or link).
Challenge Level: Hard—link form to table preview (e.g., stock output ties to inventory data), manual validation of 15+ inputs. Time: 5-7 hours. Test: Tab quiz flow, WAVE check. Output: enhanced-contact.html, commit "Day-1-2-Recipe-Enhance".

Why Best: Evolves basic form into content hub (like AllRecipes admin), blending files for practical mastery—preps for CSS styling next. Commit to repo; Day-003 awaits!
