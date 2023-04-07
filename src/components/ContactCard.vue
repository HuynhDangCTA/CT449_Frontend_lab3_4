<template>
    <div>
      <div class="p-1">
        <strong>Tên:</strong>
        {{ contact.name }}
      </div>
      <div class="p-1">
        <strong>E-mail:</strong>
        {{ contact.email }}
      </div>
      <div class="p-1">
        <strong>Địa chỉ:</strong>
        {{ contact.address }}
      </div>
      <div class="p-1">
        <strong>Điện thoại:</strong>
        {{ contact.phone }}
      </div>
      <div class="p-1">
        <strong>Liên hệ yêu thích:</strong>
        <i :class="{'fas fa-check': contact.favorite, 'fas fa-times': !contact.favorite}"></i>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      contact: {
        type: Object,
        required: true
      }
    }
  };
  </script>
  