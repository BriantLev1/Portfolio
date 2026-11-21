<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Briant Woolley - Portfolio</title>
    <link rel="preload" href="fonts/space-grotesk-latin-wght-normal.woff2" as="font" type="font/woff2" crossorigin>
    <script src="js/theme-preference.js"></script>
    <link rel="stylesheet" href="css/main.css">
</head>
<body>
    <header class="board-header">
        <details class="theme-menu">
            <summary class="theme-control">
                <span class="visually-hidden">Color scheme</span>
            </summary>
            <div class="theme-extra" role="group" aria-label="Choose color scheme">
                <label class="theme-control theme-pick" data-theme-pick="light">
                    <input name="theme-preference" type="radio" value="light">
                    <span aria-hidden="true">&#9788;&#65039;</span>
                    <span class="visually-hidden">Light</span>
                </label>
                <label class="theme-control theme-pick" data-theme-pick="system">
                    <input name="theme-preference" type="radio" value="system" checked>
                    <span aria-hidden="true">&#9881;&#65039;</span>
                    <span class="visually-hidden">System default</span>
                </label>
                <label class="theme-control theme-pick" data-theme-pick="dark">
                    <input name="theme-preference" type="radio" value="dark">
                    <span aria-hidden="true">&#127766;</span>
                    <span class="visually-hidden">Dark</span>
                </label>
            </div>
        </details>
        <h1>Briant Woolley</h1>
        <p>WDD 331R Advanced CSS</p>
        <p>
            Hello, I am from a small town in Arizona called Seligman. I am currently a student at
            BYU-Idaho studying Software Engineering. The purpose of this website is to present my
            projects and skills to potential employers. I have a big drive to learn as much as I can
            and to gain experience as a Software Developer.
        </p>
    </header>

    <main>
        <section class="card-group">
            <h2>Assignments</h2>
            <div class="cards">
                <article class="card">
                    <span class="card-tag">Unit 1</span>
                    <h3>Custom Properties and Nesting</h3>
                    <p>Design tokens built with CSS custom properties and organized with native nesting.</p>
                    <div class="card-meta">
                        <span>Assignment</span>
                        <a href="unit-1/custom-properties/index.html">View<span class="visually-hidden"> Custom Properties and Nesting</span></a>
                    </div>
                </article>

                <article class="card">
                    <span class="card-tag">Unit 2</span>
                    <h3>Layered Components</h3>
                    <p>Components organized with cascade layers so the order of styles stays predictable.</p>
                    <div class="card-meta">
                        <span>Assignment</span>
                        <a href="unit-2/layered-components/index.html">View<span class="visually-hidden"> Layered Components</span></a>
                    </div>
                </article>

                <article class="card">
                    <span class="card-tag">Unit 4</span>
                    <h3>Editorial Layout</h3>
                    <p>A long-form article page laid out with grid-template-areas that stacks on small screens and adds a fixed-width sidebar on wider ones.</p>
                    <div class="card-meta">
                        <span>Assignment</span>
                        <a href="unit-4/grid-layouts/editorial.html">View<span class="visually-hidden"> Editorial Layout</span></a>
                    </div>
                </article>

                <article class="card">
                    <span class="card-tag">Unit 4</span>
                    <h3>Responsive Card Grid</h3>
                    <p>A card grid built with auto-fit and minmax(min()) that never overflows, with read-more links pinned to the bottom of each card.</p>
                    <div class="card-meta">
                        <span>Assignment</span>
                        <a href="unit-4/grid-layouts/cards.html">View<span class="visually-hidden"> Responsive Card Grid</span></a>
                    </div>
                </article>

                <article class="card">
                    <span class="card-tag">Unit 4</span>
                    <h3>Container Queries</h3>
                    <p>One card component placed in a narrow sidebar and a wide main area, rearranging itself with named @container rules and no media queries or JavaScript.</p>
                    <div class="card-meta">
                        <span>Assignment</span>
                        <a href="unit-4/advanced/container-demo.html">View<span class="visually-hidden"> Container Queries</span></a>
                    </div>
                </article>

                <article class="card">
                    <span class="card-tag">Unit 4</span>
                    <h3>Sticky Positioning</h3>
                    <p>A sticky table of contents and section headings, including the overflow: hidden bug that silently breaks sticky and the overflow: clip fix.</p>
                    <div class="card-meta">
                        <span>Assignment</span>
                        <a href="unit-4/advanced/sticky-demo.html">View<span class="visually-hidden"> Sticky Positioning</span></a>
                    </div>
                </article>

                <article class="card">
                    <span class="card-tag">Print</span>
                    <h3>Resume and Print Stylesheet</h3>
                    <p>A resume styled with the site tokens on screen and a separate @media print block that prints cleanly to PDF.</p>
                    <div class="card-meta">
                        <span>Assignment</span>
                        <a href="unit-5/resume/resume.html">View<span class="visually-hidden"> Resume and Print Stylesheet</span></a>
                    </div>
                </article>

                <article class="card">
                    <span class="card-tag">Forms</span>
                    <h3>Contact Form</h3>
                    <p>An accessible contact form with labeled fields, a brand-colored checkbox, and a textarea that grows with field-sizing.</p>
                    <div class="card-meta">
                        <span>Assignment</span>
                        <a href="unit-5/contact/contact.html">View<span class="visually-hidden"> Contact Form</span></a>
                    </div>
                </article>
            </div>
        </section>

        <section class="card-group">
            <h2>Choose Topics</h2>
            <div class="cards">
                <article class="card">
                    <span class="card-tag">Unit 2</span>
                    <h3>::part() and ::slotted()</h3>
                    <p>A Web Component demo showing how to style Shadow DOM content with ::part() and ::slotted().</p>
                    <div class="card-meta">
                        <span>Choose topic</span>
                        <a href="unit-2/part-and-slotted/index.html">View<span class="visually-hidden"> ::part() and ::slotted()</span></a>
                    </div>
                </article>

                <article class="card">
                    <span class="card-tag">Unit 3</span>
                    <h3>Visual effects</h3>
                    <p>Layered shadows, gradient overlays, image filters, and a frosted glass panel that work in light and dark mode.</p>
                    <div class="card-meta">
                        <span>Choose topic</span>
                        <a href="unit-3/visual-effects/index.html">View<span class="visually-hidden"> Visual effects</span></a>
                    </div>
                </article>

                <article class="card">
                    <span class="card-tag">Unit 4</span>
                    <h3>display: contents</h3>
                    <p>Flattening a plain card wrapper out of the layout tree so its children join the card's grid, with the accessibility tradeoffs considered.</p>
                    <div class="card-meta">
                        <span>Choose topic</span>
                        <a href="unit-4/grid-layouts/cards.html">View<span class="visually-hidden"> display: contents</span></a>
                    </div>
                </article>

                <article class="card">
                    <span class="card-tag">Unit 5</span>
                    <h3>Variable Font Axis</h3>
                    <p>Demonstrating how to use variable font axes in CSS for dynamic typography.</p>
                    <div class="card-meta">
                        <span>Choose topic</span>
                        <a href="choose-topics/variable-font-axes/variable-font.html">View<span class="visually-hidden"> Variable Font Axis</span></a>
                    </div>
                </article>
            </div>
        </section>
    </main>

    <footer class="board-footer">
        <p>&copy; 2026 Briant Woolley &middot; WDD 331R Advanced CSS</p>
    </footer>
</body>
</html>