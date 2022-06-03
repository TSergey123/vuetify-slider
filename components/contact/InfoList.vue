<template>
  <v-item-group class="mt-5">

    <v-item class="v-item__link">
      <a href="https://wa.me/+79161031712"
        ><img width="100" height="100" src="/whatsapp.png" alt="whatsapp"
      /></a>
    </v-item>

    <v-item class="v-item__link">
      <a href="https://t.me/+79161031712"
        ><img width="100" height="100" src="/telegram.png" alt="telegram"
      /></a>
    </v-item>

    <v-item class="v-item__link">
      <a href="mailto:toporkov123561@mail.ru"
        ><img width="100" height="100" src="/mail.png" alt="mail"
      /></a>
    </v-item>

    <v-item class="v-item__link">
      <a href="https://github.com/TSergey123"
        ><img width="100" height="100" src="/github.png" alt="github"
      /></a>
    </v-item>

    <v-item class="v-item__link">
      <a href="https://hh.ru/resume/9ae741deff02f599f40039ed1f31424d69356a"
        ><img width="100" height="100" src="/hh.png" alt="hh"
      /></a>
    </v-item>

  </v-item-group>
</template>
<script>
export default {
  name: 'InfoList',
}
</script>
<style>
@media (max-width: 555px) {
.v-item__link img {
  width: 80px;
  height: 80px;
}
}
@media (max-width: 455px) {
.v-item__link img {
  width: 60px;
  height: 60px;
}
}
@media (max-width: 355px) {
.v-item__link img {
  width: 50px;
  height: 50px;
}
}
</style>
