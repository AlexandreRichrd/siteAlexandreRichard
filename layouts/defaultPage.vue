<template>
  <Nuxt />
</template>


<style>
html{
  width: 100%;
}

body {
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100vh;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  background-color: var(--background-color);
}

:root{
  --background-color: #f1f1f1;
  --secondary-background-color: #C4C4C4;
  --portfolio-background-color: #C4C4C4;
  --sub-title-color: #7F7F7F;
  --font-color: #808080;
  --main-color: #4672E3;
}

[data-theme=darkMode]{
  --background-color: #414141;
  --secondary-background-color: #D8D8D8;
  --portfolio-background-color: #c7c8d6;
  --sub-title-color: #939393;
  --font-color: #DCDCDC;
  --main-color: #4672E3;
}

[main-color=marron]{
  --main-color: #CAB785;
  --portfolio-background-color: #d6d6c7;
}

[main-color=rouge]{
  --main-color: #C15555;
  --portfolio-background-color: #d6c7c7;
}

[main-color=violet]{
  --main-color: #9D53AF;
  --portfolio-background-color: #c7c8d6;
}

[main-color=bleu]{
  --main-color: #53AAAF;
  --portfolio-background-color: #c7d6c9;
}

[main-color=vert]{
  --main-color: #41a13e;
  --portfolio-background-color: #b9cbd1;
}

::-webkit-scrollbar {
  width: 0.3rem;
}

/* Track */
::-webkit-scrollbar-track {
  background: var(--background-color);
}
/* Handle */
::-webkit-scrollbar-thumb {
  background: #888;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #555;
}
</style>