<template>
    <div class="skill container" id="skill">
        <h1>SKILL</h1>
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
          { title: 'title1', description: 'description1', link: '', comment: 'comment1' },
          { title: 'title2', description: 'description2', link: '', comment: 'comment2' },
          { title: 'title3', description: 'description3', link: '', comment: 'comment3' },
          { title: 'title4', description: 'description4', link: '', comment: 'comment4' },
          { title: 'title5', description: 'description5', link: '', comment: 'comment5' },
          { title: 'title6', description: 'description6', link: '', comment: 'comment6' }
        ]
      }
    }
}
</script>

<style scoped>
.skill {
    height: 1000px;
    background-color: lightgreen;
}
</style>