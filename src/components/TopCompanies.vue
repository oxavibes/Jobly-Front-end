<template>
  <!-- Top Companies -->
  <div class="section-padding-top padding-bottom-90">
    <div class="container">
      <div class="row">
        <div class="col">
          <div class="section-header">
            <h2>Top Compañias</h2>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col">
          <div class="company-carousel owl-carousel">
            <top-companies-item
              :company="company"
              v-for="(company, index) in topCompanies"
              :key="index"
            >
            </top-companies-item>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- Top Companies End -->
</template>

<script>
import TopCompaniesItem from "./TopCompaniesItem";
export default {
  name: "TopCompanies",
  components: {
    TopCompaniesItem
  },
  mounted() {
    $(".company-carousel").owlCarousel({
      loop: true,
      autoplay: true,
      margin: 20,
      dots: false,
      nav: true,
      navText: [
        '<span class="ti-angle-left"></span>',
        '<span class="ti-angle-right"></span>'
      ],
      responsive: {
        0: {
          items: 1
        },
        480: {
          items: 2
        },
        768: {
          items: 3
        },
        992: {
          items: 4
        },
        1200: {
          items: 5
        }
      }
    });
  },
  data() {
    return {
      topCompanies: [
        {
          name: "Digoin",
          location: "Kansas City, Missouri",
          vacancies: "4 vacantes",
          logo: "company-logo-1.png"
        },
        {
          name: "Orion Ltd.",
          location: "Sacramento, California",
          vacancies: "2 vacantes",
          logo: "company-logo-2.png"
        },
        {
          name: "Realhouse",
          location: "London, United Kingdom",
          vacancies: "4 vacantes",
          logo: "company-logo-3.png"
        },
        {
          name: "BioPro",
          location: "Ajax, Ontarioland",
          vacancies: "4 vacantes",
          logo: "company-logo-4.png"
        },
        {
          name: "Digoin",
          location: "Kansas City, Missouri",
          vacancies: "4 Open Positions",
          logo: "company-logo-1.png"
        }
      ]
    };
  }
};
</script>

<style></style>
