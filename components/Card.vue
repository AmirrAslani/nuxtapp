<template>
    <div style="width: 260px;">
        <div class="text-right productCard" dir="rtl">
            <b-card :img-src="image" img-alt="Image" img-top
                tag="article" style="max-width: 20rem;" class="mb-2 pt-2">
                <b-card-text>{{ title }}</b-card-text>
            </b-card>
        </div>
    </div>
</template>

<script>
import 'assets/css/Card.css'
export default {
    props: ['title', 'image'],
    data() {
        return {

        }
    },
}
</script>

<style scoped>

</style>