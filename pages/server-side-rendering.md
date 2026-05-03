
###### Server-side rendering

# What changes with server-side rendering?

<div class="ssr-center">
  <p>Check the app!</p>
  <div class="demo-link-wrap">
    <a href="http://localhost:3000/ssr" target="_blank" rel="noreferrer">http://localhost:3000/ssr</a>
  </div>
</div>

<style>
.ssr-center {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  flex: 1;
  margin-top: 2rem;
}
.ssr-center p {
  margin-bottom: 1rem;
}
.demo-link-wrap {
}
a[href="http://localhost:3000/ssr"] {
  display: inline-block;
  border: 1px solid var(--deck-line);
  border-radius: 8px;
  background: var(--deck-surface);
  background-image: none;
  padding: 0.85rem 1.2rem;
  color: var(--deck-blue);
  opacity: 1;
  font-family: "JetBrains Mono", ui-monospace, SFMono-Regular, Menlo, monospace;
  font-size: 1.25rem;
  text-decoration: none;
}
a[href="http://localhost:3000/ssr"]:hover,
a[href="http://localhost:3000/ssr"]:focus {
  color: var(--deck-blue);
  background-image: none;
  text-decoration: none;
}
</style>
