<script>
export default {
  name: "TaskCard",
  props: {
    task: {
      type: Object
    },
    idx: {
      type: Number
    }
  },
  methods: {
    removeTask() {
      this.$emit('removeTask', this.idx);
    }
  }
}
</script>

<template>
    <!-- TODO: add your template code here --> 
    <div class="card" style="width: 18rem;">
    <div class="card-body">
    <h5 class="card-title">Deadline: {{ task.deadline }}</h5>
    <p class="card-text">{{ task.desc }}</p>
    <a href="#" class="btn btn-primary" @click="$emit('removeTask', idx)">Done</a>
    </div>
    </div>


     <SoundLevel></SoundLevel>
   
</template>


