<template>
    <div class="card">
      <div class="card-header">
        <slot name="header"></slot>
      </div>
      <div class="card-body">
        <slot></slot> <!-- основной контент по умолчанию -->
      </div>
      <div class="card-footer">
        <slot name="footer"></slot>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'CardComponent', // Изменено имя компонента на многословное
  };
  </script>
  
  <style scoped>
  .card {
    border: 1px solid #ccc;
    border-radius: 4px;
    margin: 10px;
    padding: 10px;
    box-shadow: 2px 2px 8px rgba(0, 0, 0, 0.1);
  }
  .card-header {
    font-size: 1.5em;
    font-weight: bold;
  }
  .card-footer {
    text-align: right;
  }
  </style>
  