<template>
    <div class="profile-item card text-center" ontouchstart="" v-on:click="reverse()">
        <div v-if="!is_reversed">
            <div class="profile-title card-header">
                {{ title }}
            </div>
            <div class="profile-body card-body p-2">
                <div v-if="this.link.length === 0">
                    {{ description }}
                </div>
                <div v-else>
                    <a :href="this.link">{{ description }}</a>
                </div>
            </div>
        </div>

        <div v-else>
            <div class="profile-title card-header text-info">
                {{ title }} 裏面
            </div>
            <div class="profile-body card-body p-2">
                {{ comment }}
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ProfileItem',
    props: {
        title: String,
        description: String,
        link: String,
        comment: String
    },
    data() {
        return {
            is_reversed: false
        }
    },
    methods: {
        reverse() {
            this.is_reversed = !this.is_reversed
        }
    }
}
</script>

<style>
.profile-item {
    filter: drop-shadow(0 5px 10px rgba(0, 0, 0, 0.6));
    margin-top: 10px;
}
.profile-item:active {
    background-color: rgb(102, 102, 102);
}
</style>