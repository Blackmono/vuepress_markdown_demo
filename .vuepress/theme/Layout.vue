<template>
  <div id="app-root">
    <main>
      <p class="meta">This content will be rendered:</p>
      <Content/>
    </main>
    <aside>
      <p class="meta">This content will not:</p>
      <article v-for="page in this.$site.pages">
        <div>{{ page.title }}</div>
        <div>{{ page.excerpt }}</div>
      </article>
    </aside>
  </div>
</template>

<style>
.meta {
  background: black;
  color: white;
  margin: 1em 0;
  padding: 1em;
}
</style>

