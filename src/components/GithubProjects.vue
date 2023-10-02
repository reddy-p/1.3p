<template>
  <div class="github-projects">
    <h3>SIT120</h3>
    <h2>My Gitub projects from this semester: </h2>
    <p></p>
    <ul>
      <li v-for="repo in githubRepos" :key="repo.id">
        <a :href="repo.html_url" target="_blank">
          {{ repo.name }}
        </a>
        <p>{{ repo.description }}</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      githubRepos: [
        {
          id: 1,
          name: 'Project 1.1P',
          html_url: 'https://github.com/reddy-p/1.1P',
          description: 'Introduction to Web Apps: in this project we learnt the basics of HTML and CSS. We then created a github account and pushed code we had written to it.',
        },
        {
          id: 2,
          name: 'Project 1.2P',
          html_url: 'https://github.com/reddy-p/1.2p',
          description: 'Intoduction to Responsive Web Apps: In this task we learnt about responsive web deign. This means that it will automatically scale and look good on different size screens and can be important for accessiblity',
        },
        {
          id: 3,
          name: 'Project 1.3P',
          html_url: 'https://github.com/reddy-p/1.3p',
          description: 'Personal Portfolio... this site!',
        },
      ],
    };
  },
};
</script>

<style scoped>
.github-projects {
  max-width: 800px;
  margin: 0 auto;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  margin-bottom: 20px;
}

a {
  text-decoration: none;
  color: #0073e6;
  font-weight: bold;
}

a:hover {
  text-decoration: underline;
}
</style>
