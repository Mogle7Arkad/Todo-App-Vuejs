<template>
    <div class="container">
        <Header title="Todo App"/>
    </div>
</template>

<script>
    import Header from './components/Header.vue'
    export default {
      name: 'App',
      components: {
          Header
      },
      data() {
        return {
          tasks:[]
        }
      },
      created() {
        this.tasks = [
          {
            id: 1,
            text: 'Appointment',
            day: 'June 15th at 2:30pm',
            reminder: true,
          },
          {
            id: 2,
            text: 'zoom meeting',
            day: 'June 19th at 11:30am',
            reminder: false,
          },
          {
            id: 3,
            text: 'Church',
            day: 'June 22nd at 4:30pm',
            reminder: true,
          },
          {
            id: 4,
            text: 'Gym',
            day: 'June 23rd at 5:00pm',
            reminder: false,
          },
        ]
      }
    }
</script>

<style>
      @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400&display=swap');

    * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    }

    body {
    font-family: 'Poppins', sans-serif;
    }

    .container {
    max-width: 500px;
    margin: 30px auto;
    overflow: auto;
    min-height: 300px;
    border: 1px solid steelblue;
    padding: 30px;
    border-radius: 5px;
    }

  .btn {
    display: inline-block;
    background: #000;
    color: #fff;
    border: none;
    padding: 10px 20px;
    margin: 5px;
    border-radius: 5px;
    cursor: pointer;
    text-decoration: none;
    font-size: 15px;
    font-family: inherit;
  }

</style>