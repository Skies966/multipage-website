<template>
  <div>
    <p v-if="$fetchState.pending">Loading....</p>
    <p v-else-if="$fetchState.error">Error while fetching mountains</p>
    <div v-else>
      <h1>The <a href="https://carbon-intensity.github.io/api-definitions/#carbon-intensity-api-v2-0-0" target="_blank" >Official Carbon Intensity API</a> developed by National Grid </h1>
      
      <p>
        Region: {{ story.data[0].shortname }}
      </p>
      <p>
        Date: From {{ story.data[0].data[0].from }} --- To {{ story.data[0].data[0].to }}
      </p>
      <p>
        Forecast: {{ story.data[0].data[0].intensity.forecast }} gCO2 per kWh
      </p>
        <p>
        Index: {{ story.data[0].data[0].intensity.index }}
      </p>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        story: []
      }
    },
    async fetch() {
      this.story = await fetch(
        'https://api.carbonintensity.org.uk/regional/england'
      ).then(res => res.json())
    }
  }

  

</script>

<style>

</style>