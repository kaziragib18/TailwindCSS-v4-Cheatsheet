<!-- README: Tailwind CSS v4 Master Cheatsheet (HTML for GitHub README) -->
<h1 align="center">🌪️ Tailwind CSS v4 — Master Cheatsheet</h1>
<p align="center">
  <strong>Complete reference + learning guide (Beginner → Advanced)</strong><br/>
  Tailwind utilities mapped to CSS equivalents (default theme). Paste into your <code>README.md</code>.
</p>

<hr/>

<section>
  <h2>🎯 What is Tailwind CSS?</h2>
  <p>
    Tailwind is a <strong>utility-first CSS framework</strong>. Instead of writing bespoke CSS, you compose small, single-purpose utility classes in your HTML.
    This yields speed, consistency, and fewer context-switches. Think in <em>layout primitives</em> (display, spacing, typography, color).
  </p>
  <blockquote>
    <strong>Why it works:</strong> predictable naming and a design token system (spacing, colors, fonts) let you build UIs fast and keep them consistent.
  </blockquote>
</section>

<hr/>

<section>
  <h2>📚 Learning Roadmap</h2>
  <ol>
    <li><strong>Beginner</strong> — layout, spacing, typography, colors.</li>
    <li><strong>Intermediate</strong> — flex/grid patterns, responsive prefixes, state variants.</li>
    <li><strong>Advanced</strong> — theming, plugins, <code>@apply</code>, performance (purge), component extraction, CVA/clsx patterns.</li>
  </ol>
</section>

<hr/>

<!-- Layout & Display -->
<section>
  <h2>🧱 Layout & Display</h2>
  <p><em>Control element display and overflow.</em></p>
  <table>
    <thead>
      <tr><th align="left">Class</th><th align="left">CSS Equivalent</th></tr>
    </thead>
    <tbody>
      <tr><td><code>.block</code></td><td><code>display: block;</code></td></tr>
      <tr><td><code>.inline</code></td><td><code>display: inline;</code></td></tr>
      <tr><td><code>.inline-block</code></td><td><code>display: inline-block;</code></td></tr>
      <tr><td><code>.flex</code></td><td><code>display: flex;</code></td></tr>
      <tr><td><code>.inline-flex</code></td><td><code>display: inline-flex;</code></td></tr>
      <tr><td><code>.grid</code></td><td><code>display: grid;</code></td></tr>
      <tr><td><code>.hidden</code></td><td><code>display: none;</code></td></tr>
      <tr><td><code>.visible</code></td><td><code>visibility: visible;</code></td></tr>
      <tr><td><code>.invisible</code></td><td><code>visibility: hidden;</code></td></tr>
      <tr><td><code>.overflow-hidden</code></td><td><code>overflow: hidden;</code></td></tr>
      <tr><td><code>.overflow-auto</code></td><td><code>overflow: auto;</code></td></tr>
      <tr><td><code>.overflow-scroll</code></td><td><code>overflow: scroll;</code></td></tr>
      <tr><td><code>.overflow-x-auto</code></td><td><code>overflow-x: auto;</code></td></tr>
      <tr><td><code>.overflow-y-auto</code></td><td><code>overflow-y: auto;</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Positioning -->
<section>
  <h2>📍 Positioning</h2>
  <p><em>Shorthand for CSS positioning and offsets.</em></p>
  <table>
    <thead><tr><th align="left">Class</th><th align="left">CSS Equivalent</th></tr></thead>
    <tbody>
      <tr><td><code>.static</code></td><td><code>position: static;</code></td></tr>
      <tr><td><code>.relative</code></td><td><code>position: relative;</code></td></tr>
      <tr><td><code>.absolute</code></td><td><code>position: absolute;</code></td></tr>
      <tr><td><code>.fixed</code></td><td><code>position: fixed;</code></td></tr>
      <tr><td><code>.sticky</code></td><td><code>position: sticky;</code></td></tr>
      <tr><td><code>.inset-0</code></td><td><code>top: 0; right: 0; bottom: 0; left: 0;</code></td></tr>
      <tr><td><code>.inset-x-0</code></td><td><code>left: 0; right: 0;</code></td></tr>
      <tr><td><code>.inset-y-0</code></td><td><code>top: 0; bottom: 0;</code></td></tr>
      <tr><td><code>.top-0</code></td><td><code>top: 0;</code></td></tr>
      <tr><td><code>.right-0</code></td><td><code>right: 0;</code></td></tr>
      <tr><td><code>.bottom-0</code></td><td><code>bottom: 0;</code></td></tr>
      <tr><td><code>.left-0</code></td><td><code>left: 0;</code></td></tr>
      <tr><td><code>.top-1</code></td><td><code>top: 0.25rem; /* 4px */</code></td></tr>
      <tr><td><code>.top-2</code></td><td><code>top: 0.5rem;  /* 8px */</code></td></tr>
      <tr><td><code>.top-4</code></td><td><code>top: 1rem;    /* 16px */</code></td></tr>
      <tr><td><code>.top-8</code></td><td><code>top: 2rem;    /* 32px */</code></td></tr>
      <tr><td><code>.z-0</code></td><td><code>z-index: 0;</code></td></tr>
      <tr><td><code>.z-10</code></td><td><code>z-index: 10;</code></td></tr>
      <tr><td><code>.z-20</code></td><td><code>z-index: 20;</code></td></tr>
      <tr><td><code>.z-30</code></td><td><code>z-index: 30;</code></td></tr>
      <tr><td><code>.z-40</code></td><td><code>z-index: 40;</code></td></tr>
      <tr><td><code>.z-50</code></td><td><code>z-index: 50;</code></td></tr>
      <tr><td><code>.z-auto</code></td><td><code>z-index: auto;</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Spacing -->
<section>
  <h2>📐 Spacing (Margin & Padding)</h2>
  <p><em>Tailwind spacing scale (selected):</em> <code>0 → 0</code>, <code>px → 1px</code>, <code>0.5 → 0.125rem</code>, <code>1 → 0.25rem</code>, <code>1.5 → 0.375rem</code>, <code>2 → 0.5rem</code>, <code>2.5 → 0.625rem</code>, <code>3 → 0.75rem</code>, <code>3.5 → 0.875rem</code>, <code>4 → 1rem</code>, <code>5 → 1.25rem</code>, <code>6 → 1.5rem</code>, <code>8 → 2rem</code>, <code>10 → 2.5rem</code>, <code>12 → 3rem</code>, <code>16 → 4rem</code>, <code>20 → 5rem</code>, <code>24 → 6rem</code>, <code>32 → 8rem</code>.</p>

  <table>
    <thead><tr><th align="left">Class</th><th align="left">CSS Equivalent</th></tr></thead>
    <tbody>
      <tr><td><code>.m-0</code></td><td><code>margin: 0;</code></td></tr>
      <tr><td><code>.m-px</code></td><td><code>margin: 1px;</code></td></tr>
      <tr><td><code>.m-4</code></td><td><code>margin: 1rem;</code></td></tr>
      <tr><td><code>.mx-4</code></td><td><code>margin-left: 1rem; margin-right: 1rem;</code></td></tr>
      <tr><td><code>.my-2</code></td><td><code>margin-top: 0.5rem; margin-bottom: 0.5rem;</code></td></tr>
      <tr><td><code>.mt-6</code></td><td><code>margin-top: 1.5rem;</code></td></tr>
      <tr><td><code>.mr-3</code></td><td><code>margin-right: 0.75rem;</code></td></tr>
      <tr><td><code>.mb-8</code></td><td><code>margin-bottom: 2rem;</code></td></tr>
      <tr><td><code>.ml-1.5</code></td><td><code>margin-left: 0.375rem;</code></td></tr>
      <tr><td><code>.mx-auto</code></td><td><code>margin-left: auto; margin-right: auto;</code></td></tr>
      <tr><td><code>.-mt-4</code></td><td><code>margin-top: -1rem;</code></td></tr>
      <tr><td><code>.p-4</code></td><td><code>padding: 1rem;</code></td></tr>
      <tr><td><code>.px-6</code></td><td><code>padding-left: 1.5rem; padding-right: 1.5rem;</code></td></tr>
      <tr><td><code>.py-2.5</code></td><td><code>padding-top: 0.625rem; padding-bottom: 0.625rem;</code></td></tr>
      <tr><td><code>.pt-3</code></td><td><code>padding-top: 0.75rem;</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Flexbox -->
<section>
  <h2>🔲 Flexbox</h2>
  <p><em>Primary flex utilities for layout and alignment.</em></p>
  <table>
    <thead><tr><th align="left">Class</th><th align="left">CSS Equivalent</th></tr></thead>
    <tbody>
      <tr><td><code>.flex-row</code></td><td><code>flex-direction: row;</code></td></tr>
      <tr><td><code>.flex-row-reverse</code></td><td><code>flex-direction: row-reverse;</code></td></tr>
      <tr><td><code>.flex-col</code></td><td><code>flex-direction: column;</code></td></tr>
      <tr><td><code>.flex-col-reverse</code></td><td><code>flex-direction: column-reverse;</code></td></tr>
      <tr><td><code>.flex-wrap</code></td><td><code>flex-wrap: wrap;</code></td></tr>
      <tr><td><code>.flex-nowrap</code></td><td><code>flex-wrap: nowrap;</code></td></tr>
      <tr><td><code>.flex-wrap-reverse</code></td><td><code>flex-wrap: wrap-reverse;</code></td></tr>
      <tr><td><code>.items-start</code></td><td><code>align-items: flex-start;</code></td></tr>
      <tr><td><code>.items-center</code></td><td><code>align-items: center;</code></td></tr>
      <tr><td><code>.items-end</code></td><td><code>align-items: flex-end;</code></td></tr>
      <tr><td><code>.items-stretch</code></td><td><code>align-items: stretch;</code></td></tr>
      <tr><td><code>.items-baseline</code></td><td><code>align-items: baseline;</code></td></tr>
      <tr><td><code>.justify-start</code></td><td><code>justify-content: flex-start;</code></td></tr>
      <tr><td><code>.justify-center</code></td><td><code>justify-content: center;</code></td></tr>
      <tr><td><code>.justify-end</code></td><td><code>justify-content: flex-end;</code></td></tr>
      <tr><td><code>.justify-between</code></td><td><code>justify-content: space-between;</code></td></tr>
      <tr><td><code>.justify-around</code></td><td><code>justify-content: space-around;</code></td></tr>
      <tr><td><code>.justify-evenly</code></td><td><code>justify-content: space-evenly;</code></td></tr>
      <tr><td><code>.content-start</code></td><td><code>align-content: flex-start;</code></td></tr>
      <tr><td><code>.content-center</code></td><td><code>align-content: center;</code></td></tr>
      <tr><td><code>.content-end</code></td><td><code>align-content: flex-end;</code></td></tr>
      <tr><td><code>.content-between</code></td><td><code>align-content: space-between;</code></td></tr>
      <tr><td><code>.content-around</code></td><td><code>align-content: space-around;</code></td></tr>
      <tr><td><code>.content-evenly</code></td><td><code>align-content: space-evenly;</code></td></tr>
      <tr><td><code>.gap-0</code></td><td><code>gap: 0;</code></td></tr>
      <tr><td><code>.gap-2</code></td><td><code>gap: 0.5rem;</code></td></tr>
      <tr><td><code>.gap-4</code></td><td><code>gap: 1rem;</code></td></tr>
      <tr><td><code>.gap-x-6</code></td><td><code>column-gap: 1.5rem;</code></td></tr>
      <tr><td><code>.gap-y-3</code></td><td><code>row-gap: 0.75rem;</code></td></tr>
      <tr><td><code>.self-auto</code></td><td><code>align-self: auto;</code></td></tr>
      <tr><td><code>.self-start</code></td><td><code>align-self: flex-start;</code></td></tr>
      <tr><td><code>.self-center</code></td><td><code>align-self: center;</code></td></tr>
      <tr><td><code>.self-end</code></td><td><code>align-self: flex-end;</code></td></tr>
      <tr><td><code>.self-stretch</code></td><td><code>align-self: stretch;</code></td></tr>
      <tr><td><code>.flex-1</code></td><td><code>flex: 1 1 0%;</code></td></tr>
      <tr><td><code>.flex-auto</code></td><td><code>flex: 1 1 auto;</code></td></tr>
      <tr><td><code>.flex-initial</code></td><td><code>flex: 0 1 auto;</code></td></tr>
      <tr><td><code>.flex-none</code></td><td><code>flex: none;</code></td></tr>
      <tr><td><code>.grow</code></td><td><code>flex-grow: 1;</code></td></tr>
      <tr><td><code>.grow-0</code></td><td><code>flex-grow: 0;</code></td></tr>
      <tr><td><code>.shrink</code></td><td><code>flex-shrink: 1;</code></td></tr>
      <tr><td><code>.shrink-0</code></td><td><code>flex-shrink: 0;</code></td></tr>
      <tr><td><code>.order-first</code></td><td><code>order: -9999;</code></td></tr>
      <tr><td><code>.order-last</code></td><td><code>order: 9999;</code></td></tr>
      <tr><td><code>.order-none</code></td><td><code>order: 0;</code></td></tr>
      <tr><td><code>.order-1</code></td><td><code>order: 1;</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Grid -->
<section>
  <h2>🧮 Grid</h2>
  <p><em>Powerful for complex responsive layouts.</em></p>
  <table>
    <thead><tr><th align="left">Class</th><th align="left">CSS Equivalent</th></tr></thead>
    <tbody>
      <tr><td><code>.grid-cols-1</code></td><td><code>grid-template-columns: repeat(1, minmax(0, 1fr));</code></td></tr>
      <tr><td><code>.grid-cols-2</code></td><td><code>grid-template-columns: repeat(2, minmax(0, 1fr));</code></td></tr>
      <tr><td><code>.grid-cols-3</code></td><td><code>grid-template-columns: repeat(3, minmax(0, 1fr));</code></td></tr>
      <tr><td><code>.grid-cols-12</code></td><td><code>grid-template-columns: repeat(12, minmax(0, 1fr));</code></td></tr>
      <tr><td><code>.col-span-1</code></td><td><code>grid-column: span 1 / span 1;</code></td></tr>
      <tr><td><code>.col-span-3</code></td><td><code>grid-column: span 3 / span 3;</code></td></tr>
      <tr><td><code>.col-start-2</code></td><td><code>grid-column-start: 2;</code></td></tr>
      <tr><td><code>.col-end-4</code></td><td><code>grid-column-end: 4;</code></td></tr>
      <tr><td><code>.grid-rows-3</code></td><td><code>grid-template-rows: repeat(3, minmax(0, 1fr));</code></td></tr>
      <tr><td><code>.row-span-2</code></td><td><code>grid-row: span 2 / span 2;</code></td></tr>
      <tr><td><code>.gap-4</code></td><td><code>gap: 1rem;</code></td></tr>
      <tr><td><code>.gap-x-8</code></td><td><code>column-gap: 2rem;</code></td></tr>
      <tr><td><code>.gap-y-2</code></td><td><code>row-gap: 0.5rem;</code></td></tr>
      <tr><td><code>.place-items-center</code></td><td><code>place-items: center;</code></td></tr>
      <tr><td><code>.place-content-center</code></td><td><code>place-content: center;</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Sizing -->
<section>
  <h2>📐 Sizing</h2>
  <p><em>Width, max-width, height primitives.</em></p>
  <table>
    <thead><tr><th align="left">Class</th><th align="left">CSS Equivalent</th></tr></thead>
    <tbody>
      <tr><td><code>.w-0</code></td><td><code>width: 0;</code></td></tr>
      <tr><td><code>.w-px</code></td><td><code>width: 1px;</code></td></tr>
      <tr><td><code>.w-4</code></td><td><code>width: 1rem;</code></td></tr>
      <tr><td><code>.w-10</code></td><td><code>width: 2.5rem;</code></td></tr>
      <tr><td><code>.w-1/2</code></td><td><code>width: 50%;</code></td></tr>
      <tr><td><code>.w-1/3</code></td><td><code>width: 33.333333%;</code></td></tr>
      <tr><td><code>.w-2/3</code></td><td><code>width: 66.666667%;</code></td></tr>
      <tr><td><code>.w-1/4</code></td><td><code>width: 25%;</code></td></tr>
      <tr><td><code>.w-3/4</code></td><td><code>width: 75%;</code></td></tr>
      <tr><td><code>.w-full</code></td><td><code>width: 100%;</code></td></tr>
      <tr><td><code>.w-screen</code></td><td><code>width: 100vw;</code></td></tr>
      <tr><td><code>.max-w-xs</code></td><td><code>max-width: 20rem; /* 320px */</code></td></tr>
      <tr><td><code>.max-w-sm</code></td><td><code>max-width: 24rem; /* 384px */</code></td></tr>
      <tr><td><code>.max-w-md</code></td><td><code>max-width: 28rem; /* 448px */</code></td></tr>
      <tr><td><code>.max-w-lg</code></td><td><code>max-width: 32rem; /* 512px */</code></td></tr>
      <tr><td><code>.max-w-xl</code></td><td><code>max-width: 36rem; /* 576px */</code></td></tr>
      <tr><td><code>.max-w-2xl</code></td><td><code>max-width: 42rem; /* 672px */</code></td></tr>
      <tr><td><code>.max-w-4xl</code></td><td><code>max-width: 56rem; /* 896px */</code></td></tr>
      <tr><td><code>.max-w-7xl</code></td><td><code>max-width: 80rem; /* 1280px */</code></td></tr>
      <tr><td><code>.h-0</code></td><td><code>height: 0;</code></td></tr>
      <tr><td><code>.h-px</code></td><td><code>height: 1px;</code></td></tr>
      <tr><td><code>.h-4</code></td><td><code>height: 1rem;</code></td></tr>
      <tr><td><code>.h-10</code></td><td><code>height: 2.5rem;</code></td></tr>
      <tr><td><code>.h-full</code></td><td><code>height: 100%;</code></td></tr>
      <tr><td><code>.h-screen</code></td><td><code>height: 100vh;</code></td></tr>
      <tr><td><code>.min-h-screen</code></td><td><code>min-height: 100vh;</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Typography -->
<section>
  <h2>🔤 Typography</h2>
  <p><em>Font sizes, weights, alignment, line-height, tracking, colors.</em></p>
  <table>
    <thead><tr><th align="left">Class</th><th align="left">CSS Equivalent</th></tr></thead>
    <tbody>
      <tr><td><code>.text-xs</code></td><td><code>font-size: 0.75rem; line-height: 1rem;</code></td></tr>
      <tr><td><code>.text-sm</code></td><td><code>font-size: 0.875rem; line-height: 1.25rem;</code></td></tr>
      <tr><td><code>.text-base</code></td><td><code>font-size: 1rem; line-height: 1.5rem;</code></td></tr>
      <tr><td><code>.text-lg</code></td><td><code>font-size: 1.125rem; line-height: 1.75rem;</code></td></tr>
      <tr><td><code>.text-xl</code></td><td><code>font-size: 1.25rem; line-height: 1.75rem;</code></td></tr>
      <tr><td><code>.text-2xl</code></td><td><code>font-size: 1.5rem; line-height: 2rem;</code></td></tr>
      <tr><td><code>.text-3xl</code></td><td><code>font-size: 1.875rem; line-height: 2.25rem;</code></td></tr>
      <tr><td><code>.text-4xl</code></td><td><code>font-size: 2.25rem; line-height: 2.5rem;</code></td></tr>
      <tr><td><code>.text-5xl</code></td><td><code>font-size: 3rem; line-height: 1;</code></td></tr>
      <tr><td><code>.text-6xl</code></td><td><code>font-size: 3.75rem; line-height: 1;</code></td></tr>
      <tr><td><code>.font-light</code></td><td><code>font-weight: 300;</code></td></tr>
      <tr><td><code>.font-normal</code></td><td><code>font-weight: 400;</code></td></tr>
      <tr><td><code>.font-medium</code></td><td><code>font-weight: 500;</code></td></tr>
      <tr><td><code>.font-semibold</code></td><td><code>font-weight: 600;</code></td></tr>
      <tr><td><code>.font-bold</code></td><td><code>font-weight: 700;</code></td></tr>
      <tr><td><code>.italic</code></td><td><code>font-style: italic;</code></td></tr>
      <tr><td><code>.not-italic</code></td><td><code>font-style: normal;</code></td></tr>
      <tr><td><code>.text-left</code></td><td><code>text-align: left;</code></td></tr>
      <tr><td><code>.text-center</code></td><td><code>text-align: center;</code></td></tr>
      <tr><td><code>.text-right</code></td><td><code>text-align: right;</code></td></tr>
      <tr><td><code>.text-justify</code></td><td><code>text-align: justify;</code></td></tr>
      <tr><td><code>.leading-none</code></td><td><code>line-height: 1;</code></td></tr>
      <tr><td><code>.leading-tight</code></td><td><code>line-height: 1.25;</code></td></tr>
      <tr><td><code>.leading-snug</code></td><td><code>line-height: 1.375;</code></td></tr>
      <tr><td><code>.leading-normal</code></td><td><code>line-height: 1.5;</code></td></tr>
      <tr><td><code>.leading-relaxed</code></td><td><code>line-height: 1.625;</code></td></tr>
      <tr><td><code>.leading-loose</code></td><td><code>line-height: 2;</code></td></tr>
      <tr><td><code>.tracking-tighter</code></td><td><code>letter-spacing: -0.05em;</code></td></tr>
      <tr><td><code>.tracking-tight</code></td><td><code>letter-spacing: -0.025em;</code></td></tr>
      <tr><td><code>.tracking-normal</code></td><td><code>letter-spacing: 0;</code></td></tr>
      <tr><td><code>.tracking-wide</code></td><td><code>letter-spacing: 0.025em;</code></td></tr>
      <tr><td><code>.tracking-wider</code></td><td><code>letter-spacing: 0.05em;</code></td></tr>
      <tr><td><code>.tracking-widest</code></td><td><code>letter-spacing: 0.1em;</code></td></tr>
      <tr><td><code>.text-black</code></td><td><code>color: #000000;</code></td></tr>
      <tr><td><code>.text-white</code></td><td><code>color: #ffffff;</code></td></tr>
      <tr><td><code>.text-gray-500</code></td><td><code>color: #6b7280;</code></td></tr>
      <tr><td><code>.text-slate-700</code></td><td><code>color: #334155;</code></td></tr>
      <tr><td><code>.text-blue-500</code></td><td><code>color: #3b82f6;</code></td></tr>
      <tr><td><code>.text-emerald-600</code></td><td><code>color: #059669;</code></td></tr>
      <tr><td><code>.bg-white</code></td><td><code>background-color: #ffffff;</code></td></tr>
      <tr><td><code>.bg-gray-100</code></td><td><code>background-color: #f3f4f6;</code></td></tr>
      <tr><td><code>.bg-slate-900</code></td><td><code>background-color: #0f172a;</code></td></tr>
      <tr><td><code>.bg-blue-600</code></td><td><code>background-color: #2563eb;</code></td></tr>
      <tr><td><code>.bg-rose-500</code></td><td><code>background-color: #f43f5e;</code></td></tr>
      <tr><td><code>.decoration-sky-500</code></td><td><code>text-decoration-color: #0ea5e9;</code></td></tr>
      <tr><td><code>.underline</code></td><td><code>text-decoration-line: underline;</code></td></tr>
      <tr><td><code>.no-underline</code></td><td><code>text-decoration-line: none;</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Borders & Radius -->
<section>
  <h2>🖼️ Borders & Radius</h2>
  <table>
    <thead><tr><th align="left">Class</th><th align="left">CSS Equivalent</th></tr></thead>
    <tbody>
      <tr><td><code>.border</code></td><td><code>border-width: 1px;</code></td></tr>
      <tr><td><code>.border-0</code></td><td><code>border-width: 0;</code></td></tr>
      <tr><td><code>.border-2</code></td><td><code>border-width: 2px;</code></td></tr>
      <tr><td><code>.border-4</code></td><td><code>border-width: 4px;</code></td></tr>
      <tr><td><code>.border-t</code></td><td><code>border-top-width: 1px;</code></td></tr>
      <tr><td><code>.border-x-2</code></td><td><code>border-left-width: 2px; border-right-width: 2px;</code></td></tr>
      <tr><td><code>.border-solid</code></td><td><code>border-style: solid;</code></td></tr>
      <tr><td><code>.border-dashed</code></td><td><code>border-style: dashed;</code></td></tr>
      <tr><td><code>.border-dotted</code></td><td><code>border-style: dotted;</code></td></tr>
      <tr><td><code>.border-gray-200</code></td><td><code>border-color: #e5e7eb;</code></td></tr>
      <tr><td><code>.border-slate-700</code></td><td><code>border-color: #334155;</code></td></tr>
      <tr><td><code>.border-blue-500</code></td><td><code>border-color: #3b82f6;</code></td></tr>
      <tr><td><code>.rounded-none</code></td><td><code>border-radius: 0;</code></td></tr>
      <tr><td><code>.rounded-sm</code></td><td><code>border-radius: 0.125rem;</code></td></tr>
      <tr><td><code>.rounded</code></td><td><code>border-radius: 0.25rem;</code></td></tr>
      <tr><td><code>.rounded-md</code></td><td><code>border-radius: 0.375rem;</code></td></tr>
      <tr><td><code>.rounded-lg</code></td><td><code>border-radius: 0.5rem;</code></td></tr>
      <tr><td><code>.rounded-xl</code></td><td><code>border-radius: 0.75rem;</code></td></tr>
      <tr><td><code>.rounded-2xl</code></td><td><code>border-radius: 1rem;</code></td></tr>
      <tr><td><code>.rounded-3xl</code></td><td><code>border-radius: 1.5rem;</code></td></tr>
      <tr><td><code>.rounded-full</code></td><td><code>border-radius: 9999px;</code></td></tr>
      <tr><td><code>.rounded-t-lg</code></td><td><code>border-top-left-radius: 0.5rem; border-top-right-radius: 0.5rem;</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Shadows, Rings, Filters -->
<section>
  <h2>✨ Shadows, Rings & Filters</h2>
  <p><em>Shadows and visual filters for depth and polish.</em></p>
  <table>
    <thead><tr><th align="left">Class</th><th align="left">CSS Equivalent</th></tr></thead>
    <tbody>
      <tr><td><code>.shadow-sm</code></td><td><code>box-shadow: 0 1px 2px 0 rgb(0 0 0 / 0.05);</code></td></tr>
      <tr><td><code>.shadow</code></td><td><code>box-shadow: 0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);</code></td></tr>
      <tr><td><code>.shadow-md</code></td><td><code>box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);</code></td></tr>
      <tr><td><code>.shadow-lg</code></td><td><code>box-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);</code></td></tr>
      <tr><td><code>.shadow-xl</code></td><td><code>box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);</code></td></tr>
      <tr><td><code>.shadow-2xl</code></td><td><code>box-shadow: 0 25px 50px -12px rgb(0 0 0 / 0.25);</code></td></tr>
      <tr><td><code>.shadow-inner</code></td><td><code>box-shadow: inset 0 2px 4px 0 rgb(0 0 0 / 0.05);</code></td></tr>
      <tr><td><code>.shadow-none</code></td><td><code>box-shadow: 0 0 #0000;</code></td></tr>
      <tr><td><code>.ring</code></td><td><code>box-shadow: 0 0 0 3px rgb(59 130 246 / 0.5);</code></td></tr>
      <tr><td><code>.ring-2</code></td><td><code>box-shadow: 0 0 0 2px currentColor;</code></td></tr>
      <tr><td><code>.ring-4</code></td><td><code>box-shadow: 0 0 0 4px currentColor;</code></td></tr>
      <tr><td><code>.ring-offset-2</code></td><td><code>box-shadow: 0 0 0 2px #fff, 0 0 0 calc(2px + var(--tw-ring-offset-width, 0px)) currentColor;</code></td></tr>
      <tr><td><code>.blur-sm</code></td><td><code>filter: blur(4px);</code></td></tr>
      <tr><td><code>.blur</code></td><td><code>filter: blur(8px);</code></td></tr>
      <tr><td><code>.blur-lg</code></td><td><code>filter: blur(16px);</code></td></tr>
      <tr><td><code>.brightness-110</code></td><td><code>filter: brightness(1.1);</code></td></tr>
      <tr><td><code>.contrast-125</code></td><td><code>filter: contrast(1.25);</code></td></tr>
      <tr><td><code>.grayscale</code></td><td><code>filter: grayscale(100%);</code></td></tr>
      <tr><td><code>.hue-rotate-60</code></td><td><code>filter: hue-rotate(60deg);</code></td></tr>
      <tr><td><code>.saturate-150</code></td><td><code>filter: saturate(1.5);</code></td></tr>
      <tr><td><code>.sepia</code></td><td><code>filter: sepia(100%);</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Transitions & Transforms -->
<section>
  <h2>🔄 Transitions & Transforms</h2>
  <p><em>Animation and transform primitives (note: many set CSS vars internally).</em></p>
  <table>
    <thead><tr><th align="left">Class</th><th align="left">CSS Equivalent</th></tr></thead>
    <tbody>
      <tr><td><code>.transition</code></td><td><code>transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, backdrop-filter; transition-duration: 150ms; transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);</code></td></tr>
      <tr><td><code>.transition-colors</code></td><td><code>transition-property: color, background-color, border-color, text-decoration-color, fill, stroke;</code></td></tr>
      <tr><td><code>.transition-opacity</code></td><td><code>transition-property: opacity;</code></td></tr>
      <tr><td><code>.duration-75</code></td><td><code>transition-duration: 75ms;</code></td></tr>
      <tr><td><code>.duration-150</code></td><td><code>transition-duration: 150ms;</code></td></tr>
      <tr><td><code>.duration-300</code></td><td><code>transition-duration: 300ms;</code></td></tr>
      <tr><td><code>.ease-linear</code></td><td><code>transition-timing-function: linear;</code></td></tr>
      <tr><td><code>.ease-in</code></td><td><code>transition-timing-function: cubic-bezier(0.4, 0, 1, 1);</code></td></tr>
      <tr><td><code>.ease-out</code></td><td><code>transition-timing-function: cubic-bezier(0, 0, 0.2, 1);</code></td></tr>
      <tr><td><code>.ease-in-out</code></td><td><code>transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);</code></td></tr>
      <tr><td><code>.transform</code></td><td><code>transform: translate(var(--tw-translate-x,0), var(--tw-translate-y,0)) rotate(var(--tw-rotate,0)) skewX(var(--tw-skew-x,0)) skewY(var(--tw-skew-y,0)) scaleX(var(--tw-scale-x,1)) scaleY(var(--tw-scale-y,1));</code></td></tr>
      <tr><td><code>.scale-50</code></td><td><code>--tw-scale-x: .5; --tw-scale-y: .5; transform: ...;</code></td></tr>
      <tr><td><code>.scale-95</code></td><td><code>--tw-scale-x: .95; --tw-scale-y: .95; transform: ...;</code></td></tr>
      <tr><td><code>.scale-100</code></td><td><code>--tw-scale-x: 1; --tw-scale-y: 1; transform: ...;</code></td></tr>
      <tr><td><code>.rotate-45</code></td><td><code>--tw-rotate: 45deg; transform: ...;</code></td></tr>
      <tr><td><code>.-rotate-12</code></td><td><code>--tw-rotate: -12deg; transform: ...;</code></td></tr>
      <tr><td><code>.translate-x-4</code></td><td><code>--tw-translate-x: 1rem; transform: ...;</code></td></tr>
      <tr><td><code>.-translate-y-1/2</code></td><td><code>--tw-translate-y: -50%; transform: ...;</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Opacity, Cursor, Pointer Events -->
<section>
  <h2>🎯 Opacity, Cursor, Pointer Events, Selection</h2>
  <table>
    <thead><tr><th align="left">Class</th><th align="left">CSS Equivalent</th></tr></thead>
    <tbody>
      <tr><td><code>.opacity-0</code></td><td><code>opacity: 0;</code></td></tr>
      <tr><td><code>.opacity-50</code></td><td><code>opacity: 0.5;</code></td></tr>
      <tr><td><code>.opacity-100</code></td><td><code>opacity: 1;</code></td></tr>
      <tr><td><code>.cursor-pointer</code></td><td><code>cursor: pointer;</code></td></tr>
      <tr><td><code>.cursor-not-allowed</code></td><td><code>cursor: not-allowed;</code></td></tr>
      <tr><td><code>.pointer-events-none</code></td><td><code>pointer-events: none;</code></td></tr>
      <tr><td><code>.pointer-events-auto</code></td><td><code>pointer-events: auto;</code></td></tr>
      <tr><td><code>.select-none</code></td><td><code>user-select: none;</code></td></tr>
      <tr><td><code>.select-text</code></td><td><code>user-select: text;</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Object Fit & Backgrounds -->
<section>
  <h2>🧭 Object Fit & Backgrounds</h2>
  <table>
    <thead><tr><th align="left">Class</th><th align="left">CSS Equivalent / Notes</th></tr></thead>
    <tbody>
      <tr><td><code>.object-contain</code></td><td><code>object-fit: contain;</code></td></tr>
      <tr><td><code>.object-cover</code></td><td><code>object-fit: cover;</code></td></tr>
      <tr><td><code>.object-center</code></td><td><code>object-position: center;</code></td></tr>
      <tr><td><code>.object-left</code></td><td><code>object-position: left;</code></td></tr>
      <tr><td><code>.bg-fixed</code></td><td><code>background-attachment: fixed;</code></td></tr>
      <tr><td><code>.bg-local</code></td><td><code>background-attachment: local;</code></td></tr>
      <tr><td><code>.bg-scroll</code></td><td><code>background-attachment: scroll;</code></td></tr>
      <tr><td><code>.bg-center</code></td><td><code>background-position: center;</code></td></tr>
      <tr><td><code>.bg-top</code></td><td><code>background-position: top;</code></td></tr>
      <tr><td><code>.bg-bottom</code></td><td><code>background-position: bottom;</code></td></tr>
      <tr><td><code>.bg-no-repeat</code></td><td><code>background-repeat: no-repeat;</code></td></tr>
      <tr><td><code>.bg-repeat-x</code></td><td><code>background-repeat: repeat-x;</code></td></tr>
      <tr><td><code>.bg-contain</code></td><td><code>background-size: contain;</code></td></tr>
      <tr><td><code>.bg-cover</code></td><td><code>background-size: cover;</code></td></tr>
      <tr><td><code>.bg-gradient-to-r</code></td><td><code>background-image: linear-gradient(to right, var(--tw-gradient-stops));</code></td></tr>
      <tr><td><code>.from-blue-500</code></td><td><code>--tw-gradient-from: #3b82f6; --tw-gradient-to: rgb(59 130 246 / 0); --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);</code></td></tr>
      <tr><td><code>.via-purple-500</code></td><td><code>--tw-gradient-via: #a855f7;</code></td></tr>
      <tr><td><code>.to-pink-500</code></td><td><code>--tw-gradient-to: #ec4899;</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Lists, Tables, Misc -->
<section>
  <h2>🧩 Lists, Tables & Misc</h2>
  <table>
    <thead><tr><th align="left">Class</th><th align="left">CSS Equivalent</th></tr></thead>
    <tbody>
      <tr><td><code>.list-disc</code></td><td><code>list-style-type: disc;</code></td></tr>
      <tr><td><code>.list-decimal</code></td><td><code>list-style-type: decimal;</code></td></tr>
      <tr><td><code>.list-none</code></td><td><code>list-style-type: none;</code></td></tr>
      <tr><td><code>.table</code></td><td><code>display: table;</code></td></tr>
      <tr><td><code>.table-fixed</code></td><td><code>table-layout: fixed;</code></td></tr>
      <tr><td><code>.border-collapse</code></td><td><code>border-collapse: collapse;</code></td></tr>
      <tr><td><code>.border-separate</code></td><td><code>border-collapse: separate;</code></td></tr>
      <tr><td><code>.align-top</code></td><td><code>vertical-align: top;</code></td></tr>
      <tr><td><code>.align-middle</code></td><td><code>vertical-align: middle;</code></td></tr>
      <tr><td><code>.align-bottom</code></td><td><code>vertical-align: bottom;</code></td></tr>
      <tr><td><code>.shadow-none</code></td><td><code>box-shadow: 0 0 #0000;</code></td></tr>
      <tr><td><code>.outline-none</code></td><td><code>outline: 2px solid transparent; outline-offset: 2px;</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Responsive & State Variants -->
<section>
  <h2>📱 Responsive & State Variants</h2>
  <p><em>How to read them:</em> Prefixed utilities create media queries using default breakpoints. State variants (hover, focus, active) create pseudo-class rules.</p>
  <table>
    <thead><tr><th align="left">Example</th><th align="left">Effect</th></tr></thead>
    <tbody>
      <tr><td><code>md:text-lg</code></td><td>Applies <code>font-size: 1.125rem;</code> at <code>min-width: 768px</code>.</td></tr>
      <tr><td><code>hover:bg-blue-600</code></td><td>On hover → <code>background-color: #2563eb;</code>.</td></tr>
      <tr><td><code>focus:ring</code></td><td>On focus → add focus ring (default blue 50% 3px).</td></tr>
    </tbody>
  </table>
  <p style="font-size:0.95em; color:#666;">Default breakpoints (v4): <code>sm</code> 640px, <code>md</code> 768px, <code>lg</code> 1024px, <code>xl</code> 1280px, <code>2xl</code> 1536px.</p>
</section>

<hr/>

<!-- Quick Recipes -->
<section>
  <h2>🧠 Quick Recipes</h2>
  <p>Common patterns you’ll use often.</p>
  <table>
    <thead><tr><th align="left">Pattern</th><th align="left">Classes / Result</th></tr></thead>
    <tbody>
      <tr><td>Center a div</td><td><code>.flex .items-center .justify-center</code> — <code>display:flex; align-items:center; justify-content:center;</code></td></tr>
      <tr><td>Card</td><td><code>.rounded-lg .shadow-md .p-6 .bg-white</code> — border-radius, shadow, padding, white bg</td></tr>
      <tr><td>Responsive grid</td><td><code>.grid .grid-cols-1 .md:grid-cols-2 .lg:grid-cols-3 .gap-6</code></td></tr>
    </tbody>
  </table>
</section>

<hr/>

<!-- Advanced Guidance -->
<section>
  <h2>⚙️ Advanced: Theming, Performance & Patterns</h2>
  <h3>theming & config</h3>
  <p>Extend <code>tailwind.config.js</code> for design tokens:</p>
  <pre><code>module.exports = {
  theme: {
    extend: {
      colors: { brand: { 50: '#f0f9ff', 500: '#0ea5e9' } },
      spacing: { 72: '18rem' },
    },
  },
};</code></pre>

  <h3>component extraction</h3>
  <p>
    For repeated patterns, extract to components (React/Vue) or use <code>@apply</code> inside CSS:
  </p>
  <pre><code>.btn-primary {
  @apply px-4 py-2 bg-blue-600 text-white rounded-md shadow;
}</code></pre>

  <h3>performance</h3>
  <ul>
    <li>Enable <code>content</code> (aka purge) so unused classes are removed in production build.</li>
    <li>Prefer semantic components + extracted classes to keep HTML manageable.</li>
  </ul>

  <h3>class management</h3>
  <p>Use utilities like <code>clsx</code> or <code>cva()</code> to compose conditional classes in JS/TS codebases.</p>
</section>

<hr/>

<!-- Pro Tips -->
<section>
  <h2>🧠 Pro Tips (Apex Developer Advisor)</h2>
  <ul>
    <li><strong>Think in Layout Primitives</strong>: Start with container & flow (display, gap, align), then refine spacing & typography.</li>
    <li><strong>Extract early</strong>: If you repeat a combination twice, make a component or utility with <code>@apply</code>.</li>
    <li><strong>Use theme tokens</strong> for brand colors and spacing. Avoid magic numbers.</li>
    <li><strong>Responsive-first</strong>: Default styles should be mobile-friendly; add breakpoints for larger screens.</li>
    <li><strong>Accessibility</strong>: Don’t rely solely on color; use focus rings, ARIA, and sufficient contrast.</li>
  </ul>
</section>

<hr/>

<!-- Footer -->
<section>
  <h2>🏁 Notes & Links</h2>
  <p>
    • Values in this cheatsheet reflect the <strong>default Tailwind v4 theme</strong>. If you customize <code>tailwind.config.js</code>, your values will differ.<br>
    • Many utilities set <code>--tw-*</code> variables that compose together (transforms, filters, rings).<br>
    • Official docs: <a href="https://tailwindcss.com/docs">https://tailwindcss.com/docs</a>
  </p>

  <p align="center">
    <em>Paste this whole HTML into your README.md — it renders cleanly on GitHub.</em>
  </p>
</section>
