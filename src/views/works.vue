<template>
    <div class="works container" id="works">
        <h1>WORKS</h1>
        <div class="card-deck row">
            <div v-for="(item, key) in profileItems" v-bind:key="key" class="col-xs-12 col-md-4">
                <profile-item v-bind="item" />
            </div>
        </div>
    </div>
</template>

<script>
import ProfileItem from '../components/ProfileItem.vue'
export default {
    components: {
        ProfileItem
    },
    data() {
      return {
        profileItems: [
          { title: 'ひらがな認識', description: 'https://mkdk09.github.io/hiragana-classification/', link: 'https://mkdk09.github.io/hiragana-classification/', comment: 'comment1' },
          { title: 'wikipedia_random', description: 'https://chlorinated-jealous-box.glitch.me/', link: 'https://chlorinated-jealous-box.glitch.me/', comment: 'comment2' },
          { title: 'dogs-vs-cats', description: 'https://mkdk09.github.io/dogs-vs-cats/', link: 'https://mkdk09.github.io/dogs-vs-cats/', comment: 'comment3' },
          { title: 'portfolio', description: 'https://mkdk09.github.io/portfolio/', link: 'https://mkdk09.github.io/portfolio/', comment: 'comment4' },
          { title: 'title5', description: 'description5', link: '', comment: 'comment5' },
          { title: 'title6', description: 'description6', link: '', comment: 'comment6' }
        ]
      }
    }
}
</script>

<style scoped>
.works {
    height: 1000px;
    background-color: lightcoral;
}
</style>