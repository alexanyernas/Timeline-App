<template>
    <v-timeline-item>
        <template v-slot:icon>
            <v-avatar color="#E1BEE7">
                <img :src="data.icon">
            </v-avatar>
        </template>
        <v-card 
            class="elevation-6" 
            color="#BA68C8" 
            dark 
            shaped 
            outlined
        >
            <v-card-title class="text-h5">
                {{ data.card_title }}
            </v-card-title>
            <v-card-text :style="{ fontSize: '20px', lineHeight: '1.25', color: '#F3E5F5' }">
                {{ data.card_content }}
            </v-card-text>
        </v-card>
    </v-timeline-item>
</template>

<script>
export default {
    name: 'TimelineItem',
    props: {
        data: Object
    }
}
</script>