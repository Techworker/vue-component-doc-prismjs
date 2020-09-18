<template>
  <div class="component-doc-prism">
    <div class="code-container">
      <pre>
        <code :class="'language-' + language">
          <slot name="code"></slot>
        </code>
      </pre>
    </div>
    <div class="result-container">
      <slot name="result"></slot>
    </div>
  </div>
</template>
<script>

export default {
  props: {
    language: {
      type: String
    }
  },
}
</script>