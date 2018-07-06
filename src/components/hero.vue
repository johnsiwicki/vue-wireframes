<template>
	<div class="heroPrompt">
		<div class="heroPrompt__item heroPromptLabel">{{headline}}</div>
		<div class="herorompt__item heroPromptDetails">{{details}}</div>
		<div class="hero__button">{{cta}}</div>
	</div>
</template>

<script>
module.exports = {
  props: ["headline", "details", "cta"],
  data: function() {
    return {};
  }
};
</script>

<style scoped>
.heroPrompt {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  min-height: 300px;
  padding: 10px;
  background-image: url(https://source.unsplash.com/random/1440x800);
  background-attachment: fixed;
  background-repeat: no-repeat;
}

.heroPromptLabel {
  color: white;
  font-size: 30px;
  font-weight: 700;
  text-align: center;
  margin: 10px 0;
}

.heroPromptDetails {
  color: white;
  font-size: 16px;
  margin-bottom: 10px;
  text-align: center;
}
.hero__button {
  display: inline-block;
  vertical-align: middle;
  margin: 0 0 1rem 0;
  padding: 0.85em 1em;
  border: 1px solid transparent;
  border-radius: 0;
  transition: background-color 0.25s ease-out, color 0.25s ease-out;
  font-size: 0.9rem;
  line-height: 1;
  text-align: center;
  cursor: pointer;
  background-color: rgb(0, 0, 0);
  color: #fefefe;
}
</style>
