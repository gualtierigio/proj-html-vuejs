<template>
    <footer>
      <div class="page-wrap">
        <div class="container">
          <div class="row gx-5">
            <FooterAbout />
            <FooterTwitter />
            <FooterLinks />
            <FooterContacts />
          </div>
        </div>
      </div>
    </footer>
</template>

<script>
import FooterAbout from './FooterAbout.vue';
import FooterTwitter from './FooterTwitter.vue';
import FooterLinks from './FooterLinks.vue';
import FooterContacts from './FooterContacts.vue';

export default {
  name: "Footer",
  components: {
    FooterAbout,
    FooterTwitter,
    FooterLinks,
    FooterContacts
  }

};
</script>


<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/variables.scss';

footer{
  background-color: $black-color-2;
  height: 50vh;
  width: 100%;
  padding-top: 100px;
}

.page-wrap{
  border: 1px solid red;
  width: 65%;
  margin: 0 auto;
}

</style>