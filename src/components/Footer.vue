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
      <div class="copyright d-flex align-items-center">
        <p>Copyright Everlead by giosby</p>
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
  width: 100%;
  padding-top: 100px;
}

.page-wrap{
  border: 1px solid red;
  width: 65%;
  margin: 0 auto;
}

.copyright{
  height: 40px;
  background-color: $red-color;
  justify-content: center;
  color: $total-white;
  opacity: 0.8;
  p{
    margin: 0;
    font-size: 0.6rem;
  }
}

</style>