<template>
    <Header>Sponsors</Header>
    <div class="sponsor-grid">
      <!-- Partner Sponsors 
      <h4><b>Partner</b></h4>
      <div class="underline"></div>
      <div class="sponsor-tier">
        <SponsorsSponsorGrid :sponslist="partnerSponsors" />
      </div> -->

         <!-- Platinum Sponsors 
      <h4><b>Platinum</b></h4>
      <div class="underline"></div>
      <div class="sponsor-tier">
        <SponsorsSponsorGrid :sponslist="platinumSponsors" />
      </div> -->

      <!-- Gold Sponsors -->
      <h4><b>Gold</b></h4>
      <div class="underline"></div>
      <div class="sponsor-tier">
        <SponsorsSponsorGrid :sponslist="goldSponsors" />
      </div>

      <!-- Silver Sponsors 
      <h4><b>Silver</b></h4>
      <div class="underline"></div>
      <div class="sponsor-tier">
        <SponsorsSponsorGrid :sponslist="silverSponsors" />
      </div> -->

      <!-- Bronze Sponsors -->
      <h4><b>Bronze</b></h4>
      <div class="underline"></div>
      <div class="sponsor-tier">
        <SponsorsSponsorGrid :sponslist="bronzeSponsors" />
      </div>

      <!-- Starter Sponsors -->
      <h4><b>Starter</b></h4>
      <div class="underline"></div>
      <div class="sponsor-tier">
        <SponsorsSponsorGrid :sponslist="starterSponsors" />
      </div>

      <!-- Custom Sponsors -->
      <h4><b>Custom</b></h4>
      <div class="underline"></div>
      <div class="sponsor-tier">
        <SponsorsSponsorGrid :sponslist="customSponsors" />
      </div>

      <!-- Virtual Sponsors -->
      <h4><b>Virtual</b></h4>
      <div class="underline"></div>
      <div class="sponsor-tier">
        <SponsorsSponsorGrid :sponslist="virtualSponsors" />
      </div>

      <!-- Special Thanks -->
      <h4><b>Special Thanks</b></h4>
      <div class="underline"></div>
      <div class="sponsor-tier">
        <SponsorsSponsorGrid :sponslist="specialThanks" />
      </div>
    </div>
</template>
  
<script setup lang="ts">
import { type SponsorInfo } from './sponsor-info';

const partnerSponsors: SponsorInfo[] = []

const platinumSponsors: SponsorInfo[] = []

const goldSponsors: SponsorInfo[] = [
  {
   name: 't-rowe-price',
   link: 'https://www.troweprice.com/corporate/us/en/home.html' 
  }
]

const silverSponsors: SponsorInfo[] = []

const bronzeSponsors: SponsorInfo[] = [
  {
    name: 'visionist',
    link: 'https://www.visionistinc.com'
  },
  {
    name: 'travelers',
    link: 'https://www.travelers.com'
  },
  {
    name: 'i4c',
    link: 'https://inclusion.cs.umd.edu/'
  }
]

const starterSponsors: SponsorInfo[] = [
  {
    name: 'softrams',
    link: 'https://www.softrams.com/'
  },

  { 
    name: 'trails',
    link: 'https://www.trails.umd.edu/'
  },
  { 
    name: 'umdbsos',
    link: 'https://bsos.umd.edu/'
  },
  { 
    name: 'tenable',
    link: 'https://www.tenable.com/'
  },
  { 
    name: 'str',
    link: 'https://str.com/'
  },

]

const customSponsors: SponsorInfo[] = [
  { 
    name: 'capital-one',
    link: 'https://www.capitalone.com/'
  },

  { 
    name: 'bloomberg-industry',
    link: 'https://www.bloombergindustry.com/'
  },

  { 
    name: 'icf',
    link: 'https://www.icf.com/'
  },

  { 
    name: '355code',
    link: 'https://www.355code.com/'
  },

  { 
    name: 'afcea',
    link: 'https://www.afcea.org/'
  },

  { 
    name: 'caci',
    link: 'https://www.caci.com/'
  },

  { 
    name: 'codepath',
    link: 'https://www.codepath.org/'
  },

  { 
    name: 'umd-cs',
    link: 'https://www.cs.umd.edu/'
  },

  { 
    name: 'umd-clark',
    link: 'https://eng.umd.edu/'
  },

  { 
    name: 'umd-sga',
    link: 'https://www.umdsga.com/'
  },

  { 
    name: 'see-funding',
    link: 'https://www.see.umd.edu/funding'
  },

  { 
    name: 'code-path',
    link: 'https://www.codepath.org'
  },
]

const virtualSponsors: SponsorInfo[] = [
  {
    name: 'qualcomm',
    link: 'https://www.qualcomm.com/'
  }
]


const specialThanks: SponsorInfo[] = [{name: "standout", link: "https://www.standoutstickers.com/"}]

</script>

<style scoped lang="scss">
.sponsor-grid {
  margin: 2rem auto;
  padding: 10px;

}

.sponsor-tier {
  margin: 1.5rem auto;
  text-align: left;
  padding-top: 0.5rem;

  display: flex;
  flex-wrap: wrap;
}

.underline {
  width: 100%;
  background-color: $LIGHTPURPLE;
  height: 0.3em;
}

.sponsor-tier img {
  width: 25%;
  padding: 2%;
}

.sponsor-tier h3 {
  margin-bottom: 0.5rem;
}

h4 {
  text-align: left;
}

</style>
