<template>
    <v-timeline
        :dense="$vuetify.breakpoint.smAndDown"
    >
        <timeline-item 
            class="my-mb" 
            v-for="( item, index ) in items" 
            :key="index"
            :data="item" 
        />
    </v-timeline>
</template>

<script>
import TimelineItem from './TimelineItem.vue'
import { textConfig } from '../config/textConfig'

export default {
    name: 'Timeline',
    components: {
        TimelineItem
    },
    data () {
        return {
            items: [ ...textConfig ]
        }
    }
}
</script>

<style scoped>
.my-mb
{    
    padding-left: 48px;
    padding-right: 48px;
}

.my-mb:not(:last-child)
{
    margin-bottom: 200px;
}

@media only screen and ( max-width: 600px ) 
{
    .my-mb
    {
        padding-left: 0;
        padding-right: 16px;
    }
}

</style>