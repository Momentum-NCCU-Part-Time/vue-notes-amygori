<script setup>
// make it easy on yourself and do small steps!
// after you get your mind around this hard coded data,
// you can change the notes variable this to a reactive value
// and make a fetch request to GET the data from the server
const notes = [
  {
    id: 1,
    title: 'Sample note',
    body: 'This is the body of my note',
    updatedAt: '2018-01-01T00:00:00.000Z',
  },
  {
    id: 2,
    title: 'Another Sample note',
    body: 'This is the body of my note',
    updatedAt: '2018-01-01T00:00:00.000Z',
  },
]
</script>

<template>
  <div>
    <h1>Vue Notes</h1>
    <ul>
      <li v-for="note in notes">
        {{ note.title }}
        {{ note.body }}
      </li>
    </ul>
  </div>
  <div>
    <form>
      <div class="form-example">
        <label for="title">Note title</label>
        // how can you work with values in inputs in Vue?
        // you can look this up in the vue documentation
        <input type="text" name="title" id="title" required />
      </div>
    </form>
  </div>
</template>

<style scoped></style>
