<template>
  <header>
      <div class="container">
        <Logo alt-text="Logo Header"/>
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :class="{active: link.current}" :href="link.url" @click.prevent="changePage(index)">{{link.text}}</a>
                </li>
            </ul>
        </nav>
      </div>
  </header>
</template>

<script>
import Logo from '../commons/Logo.vue'
export default {
    name: "Header",
    components: {
        Logo,
    },
    data() {
        return {
            links: [
                {
                    text: "Home",
                    url: "#",
                    current: false,
                },
                {
                    text: "Prodotti",
                    url: "#",
                    current: true,
                },
                {
                    text: "Chi Siamo",
                    url: "#",
                    current: false,
                },
                {
                    text: "Contatti",
                    url: "#",
                    current: false,
                },
            ]
        }
    },
    methods: {
        changePage(index) {
            this.links.forEach(link => link.current = false);
            this.links[index].current = true;
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
    header {
        text-align: center;
    }
    nav {
        ul {
            display: flex;
            justify-content: center;
            list-style: none;
            li a {
                display: inline-block;
                padding: 15px 20px;
                text-decoration: none;
                color: #000;
                &.active, &:hover {
                    background-color: $secondaryColor;
                }
            }
        }
    }
</style>