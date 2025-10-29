<script>
    //import component
    import SoundIcon from "../components/subcomponents/SoundIcon.vue"
    export default { 
        
        data() {
            return {
                soundLevel: 0
            }
        },

        components: {
            SoundIcon
        }
    }
</script>

<template>

   Sound level
    <input type="number" min="0" max="3" v-model="soundLevel"> 
    <!-- TODO: Add Code Here to make use of the component -->
     
    <sound-icon :level="soundLevel"></sound-icon>
    <!-- dynamic variable need to do the binding (:level = "soundLevel") but for static value do not need to -->
    <!--do binding (level = "soundLevel") -->

    

</template>

