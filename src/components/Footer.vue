<template>
    <footer>
      <div class="page-wrap">
        <div class="container">
          <div class="row gx-5">
            <FooterAbout />
            <FooterTwitter />
            <FooterLinks :propLinks ='links'/>
            <FooterContacts :propContacts ='contacts'/>
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
  },
  data() {
    return {
      links: [
        {
          text: "About me",
          url: "#AboutMe",
        },
        {
          text: "About us",
          url: "#AboutUs",
        },
        {
          text: "Language packs",
          url: "#LanguagePacks",
        },
        {
          text: "Become a coach",
          url: "#BecomeCoach",
        },
        {
          text: "Monthly events",
          url: "#MonthlyEvents",
        }
      ],
      contacts: [
        {
          info: "475 BigBlue Street, NY 10013",
          infoLogo: "<i class=\"fas fa-map-marker-alt\"></i>",
          url: "#address"
        },
        {
          info: "(351)5512-2579",
          infoLogo: "<i class=\"fas fa-phone-alt\"></i>",
          url: "#phone"
        },
        {
          info: "everlead@mikado.com",
          infoLogo: "<i class=\"far fa-envelope\"></i>",
          url: "#mail"
        }
      ]
    }
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
  min-width: 620px;
}

.page-wrap{
  width: 65%;
  margin: 0 auto;
}

.copyright{
  margin-top: 100px;
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