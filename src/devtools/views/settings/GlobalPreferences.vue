<template>
  <div class="global-preferences">
    <VueFormField title="Component Name Format">
      <VueGroup
        :value="$shared.classifyComponents"
        class="extend"
        @input="$shared.classifyComponents = $event"
      >
        <VueGroupButton
          :value="false"
          label="kebab-case"
        />
        <VueGroupButton
          :value="true"
          label="PascalCase"
        />
      </VueGroup>
    </VueFormField>

    <VueFormField title="Theme">
      <VueGroup
        :value="$shared.theme"
        class="extend"
        @input="$shared.theme = $event"
      >
        <VueGroupButton
          value="auto"
          label="Auto"
        />
        <VueGroupButton
          value="light"
          label="Light"
        />
        <VueGroupButton
          value="dark"
          label="Dark"
        />
      </VueGroup>
    </VueFormField>
  </div>
</template>

<style lang="stylus" scoped>
.global-preferences
  display flex
  flex-wrap wrap
  padding 1rem 1.5rem

  > *
    flex-basis 300px
    margin 0 .5rem 1rem .5rem
</style>-->
