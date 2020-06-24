<template>
  <div :class="css`text-align:center;`">
    <header :class="css`
    background-color: #f9f6f6;
  color: #32485f;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  font-size: calc(10px + 2vmin);
    `">
      <img src="/logo.svg" :class="css`
  height: 40vmin;
  pointer-events: none;
  margin-bottom: 1rem;
  animation: App-logo-spin infinite 1.6s ease-in-out alternate;

@keyframes App-logo-spin {
  from {
    transform: scale(1);
  }
  to {
    transform: scale(1.06);
  }
}
      `" alt="logo" />
      <p>
        Edit
        <code>src/App.vue</code> and save to reload.
      </p>
      <a
        :class="css`color: #00c185;`"
        href="https://vuejs.org"
        target="_blank"
        rel="noopener noreferrer"
      >{{ message }}</a>
    </header>
  </div>
</template>

<script>
import css from 'csz';
export default {
  data() {
    return {
      message: "Learn Vue",
      css
    };
  }
};

</script>
