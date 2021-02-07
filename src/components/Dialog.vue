<template>
  <div v-show="show" class="overlay">


    <div class="dialog">

      <div class="dialog__content">
        <h2 class="dialog__title" v-text="title"></h2>
        <p class="dialog__description" v-text="description"></p>
      </div>

      <hr />

      <div class="dialog__footer">
        <button @click="cancel" class="dialog__cancel">Cancel</button>
        <button @click="confirm" class="dialog__confirm">Yes, delete it</button>
      </div>

    </div>

  </div>
</template>

<script>
export default {
    props: ['show', 'title', 'description', 'cancel', 'confirm']
}
</script>
