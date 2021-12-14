<template>
  <footer>
      <div class="container">
            <Logo alt-text="Logo Footer"/>
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Veritatis officiis nihil dolores laborum earum molestias exercitationem inventore vero itaque vel incidunt ipsam, consequatur porro laudantium? Vero commodi nostrum magnam perferendis!
      </div>
  </footer>
</template>

<script>
import Logo from '../commons/Logo.vue'
export default {
    name: "Footer",
    components: {
        Logo,
    }
}
</script>

<style lang="scss" scoped>
    footer {
        background-image: url(../../assets/img/footer-montagne-bottom.jpg);
        background-position: bottom;
        background-repeat: no-repeat;
        padding: 40px 0;
    }
</style>