<template>
  <!-- we have to wrap the GL component in 'client-only'
       otherwise, Vue throws an error about SSR render mismatch -->
  <client-only>
    <golden-layout class="gl-container">
      <gl-row>
        <gl-component title="component1">
          <h1>Component 1</h1>
        </gl-component>
        <gl-stack>
          <gl-component title="component2">
            <h1>Component 2</h1>
          </gl-component>
          <gl-component title="component3">
            <h1>Component 3</h1>
          </gl-component>
        </gl-stack>
      </gl-row>
    </golden-layout>
  </client-only>
</template>
<style>
.gl-container {
  height: calc(100% - 56px);
}
</style>
