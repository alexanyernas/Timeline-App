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

export default {
    name: 'Timeline',
    components: {
        TimelineItem
    },
    data () {
        return {
            items: [
                {
                    icon: 'https://i.pravatar.cc/64',
                    icon_title: 'Tus eu perfecto',
                    card_title: 'Lorem ipsum',
                    card_content: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.'
                },
                {
                    icon: 'https://i.pravatar.cc/64',
                    icon_title: 'Tus eu perfecto',
                    card_title: 'Lorem ipsum',
                    card_content: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at.'
                },
                {
                    icon: 'https://i.pravatar.cc/64',
                    icon_title: 'Tus eu perfecto',
                    card_title: 'Lorem ipsum',
                    card_content: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at.'
                },
                {
                    icon: 'https://i.pravatar.cc/64',
                    icon_title: 'Tus eu perfecto',
                    card_title: 'Lorem ipsum',
                    card_content: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at.'
                }
            ]
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
    margin-bottom: 240px;
}

@media only screen and ( max-width: 600px ) 
{
    .my-mb
    {
        padding-left: 0;
        padding-right: 8px;
    }
}

</style>