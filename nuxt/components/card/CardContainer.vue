<template>
  <div class="card-container-body">
    <div class="products-area">
      <h1>Take a look at what global warming is doing to our Earth!</h1>
    </div>
    <div class="card-container">
      <CardContainerContent v-for="x in products" :key="x.id" :product="x"
      >
      {{x}}
      </CardContainerContent>

    </div>
   
      <img src="" alt="">
      <h3 class="attribution-title">Attributions: </h3>
     
     <div class="products-area-logo">
       <ul>
        <li>- NASA. (2022, February 8). Climate change evidence: How do we know? NASA. Retrieved April 8, 2022, from https://climate.nasa.gov/evidence/ </li>
        <li>- Macmillan, A. A. M. M. J. T., &amp; Turrentine , J. (2021, April 7). Global warming 101. NRDC. Retrieved April 8, 2022, from https://www.nrdc.org/stories/global-warming-101 </li>
        <li>- NASA. (2022, March 7). The causes of climate change. NASA. Retrieved April 8, 2022, from https://climate.nasa.gov/causes/ </li>
        <li>- Riley, T. (n.d.). 100 companies are responsible for 71% of global emissions, study says. Business &amp; Human Rights Resource Centre. Retrieved April 8, 2022, from https://www.business-humanrights.org/en/latest-news/100-companies-are-responsible-for-71-of-global-emissions-study-says/ </li>
        <li>- Palmer, M. (2021, March 7). Photo by Matt Palmer on unsplash. Beautiful Free Images &amp; Pictures. Retrieved April 8, 2022, from https://unsplash.com/photos/kbTp7dBzHyY </li>
        <li>- Hillier, J. (2019, December 20). Photo by Jason Hillier on unsplash. Beautiful Free Images &amp; Pictures. Retrieved April 8, 2022, from https://unsplash.com/photos/8aVYkPi84AY </li>
        </ul>

    </div>
  </div>
</template>

<script>
// Place content here
 export default {
    data () {
      return {
      products: [
      {
        title: 'Global Warmings Effect on Animals',
        button: 'Learn More!',
        bgtext: 'The animals on Earth have taken a toll due to global warming',
        src: require('../../assets/images/polar-bear.jpg'),
        page: ("../../animal"),
        
      },
      {
        title: 'Global Warmings Effect on the Environment',
        button: 'Learn More!',
        bgtext: 'The Environment is dying at an alarming rate, is it too late to reverse it?',
        src: require('../../assets/images/forest-burning.jpg'),
         page: ("../../environment"),
      }
    ]}
  }}
</script>

<style>


.card-container-body {
  display:flex;
  flex-direction: column;
  align-items: center;
  justify-items: center;
  text-align: center;
  gap: 1rem;

  background-color: rgba(128, 128, 128, 0.555);
  text-shadow: 3px 6px 4px rgba(0, 0, 0, 0.15);
  height: 100%;
  position: relative;
}
 .card-container {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
gap: 1.5rem;
border: 1rem;
font : 5rem;

}

.products-area-logo {
font-size:12px;
}
.products-area {

font-size:20px;

}
.attribution-title {
  font-size:18px;
}

</style>