<template>
  <Nuxt />
</template>


<style>
body {
  margin: 0;
  padding: 0;
  height: 100vh;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  background-color: var(--background-color);
}

:root{
  --background-color: #f1f1f1;
  --secondary-background-color: #C4C4C4;
  --sub-title-color: #7F7F7F;
  --font-color: #808080;
  --main-color: #4672E3;
}

[data-theme=darkMode]{
  --background-color: #373737;
  --secondary-background-color: #D8D8D8;
  --sub-title-color: #939393;
  --font-color: #DCDCDC;
  --main-color: #4672E3;
}

[main-color=marron]{
  --main-color: #CAB785;
}

[main-color=rouge]{
  --main-color: #C15555;
}

[main-color=violet]{
  --main-color: #9D53AF;
}

[main-color=bleu]{
  --main-color: #53AAAF;
}

[main-color=vert]{
  --main-color: #54AF53;
}
</style>