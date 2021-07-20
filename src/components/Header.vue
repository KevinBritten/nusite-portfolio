<template>
  <div>
    <nav>
      <ul>
        <li v-for="section in sections" :key="section">
          <a :href="'#' + section.toLowerCase()">{{ section }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      sections: [
        "Hero",
        "Mission Statement",
        "Services",
        "Work",
        "Team",
        "Blog",
        "Contact",
      ],
    };
  },
};
</script>

<style scoped>
nav {
  width: 100%;
}

ul {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  list-style-type: none;
}
li {
  padding: 0 5px;
}
a {
  display: block;
}
</style>