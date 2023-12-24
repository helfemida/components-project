<template>
    <div class="graph">
        <GraphItem class="elem" v-for="(element, index) in styles" 
            :key="index" 
            :elementName="element.elementName" 
            :backgroundColor="element.backgroundColor"
            :height="element.height"
            >
        </GraphItem>
        
    </div>
</template>

<script>
    import GraphItem from './GraphItem.vue';

    export default {
        components: {
            GraphItem
        },
       
        data() {
            return {
                styles: [
                    {elementName: 'Mon', backgroundColor: 'rgba(241,199,103,255)', height: '80%'},
                    {elementName: 'Tue', backgroundColor: 'rgba(241,199,103,255)', height: '40%'},
                    {elementName: 'Wed', backgroundColor: 'rgba(241,199,103,255)', height: '35%'},
                    {elementName: 'Thu', backgroundColor: '#ef6d4d', height: '43%'},
                    {elementName: 'Fri', backgroundColor: 'rgba(241,199,103,255)', height: '30%'}, 
                    {elementName: 'Sat', backgroundColor: 'rgba(241,199,103,255)', height: '60%'},
                    {elementName: 'Sun', backgroundColor: '#ef6d4d', height: '65%'},
                ]
            };
        },
    }
</script>

<style>
    .graph {
        width: 500px;
        height: 250px;
        display: flex;
        flex-direction: row;
        align-items: baseline;
        justify-content: space-between;
        margin: 2%;
    }
    
</style>
