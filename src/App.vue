<template>
  <div id="app">
    <h1>Пример использования слотов в Vue</h1>
    <card-component>
      <template #header>
        Заголовок карточки
      </template>

      <template #default>
        Здесь вы можете поместить любой текст или компонент, который вы хотите отобразить внутри карточки. Например, <strong>это пример текста!</strong>
      </template>

      <template #footer>
        <button @click="handleClick">Кнопка действия</button>
      </template>
    </card-component>
  </div>
</template>

<script>
import CardComponent from './components/Card.vue'; // Импортируем с новым именем

export default {
  name: 'App',
  components: {
    CardComponent,
  },
  methods: {
    handleClick() {
      alert('Кнопка нажата!');
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

