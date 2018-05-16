<template>
  <div id="app-root">

    <!-- This block will output parsed markdown -->
    <main>
      <div class="meta">CONTENT:</div>
      <Content/>
    </main>

    <!-- This block will output markdown-format plain text -->
    <aside v-for="page in this.$site.pages">
      <div class="meta">TITLE:</div>
      <div>{{ page.title }}</div>
      <div class="meta">EXCERPT:</div>
      <div>{{ page.excerpt }}</div>
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

