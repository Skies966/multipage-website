<template>
    <div>
        <TheHeader />
        <div class="environment-body">
            <h1 class="environment-title"> Global Warmings Effect on the Environment</h1>

                <p> 
                The environment is starting to die at an alarming rate. 
                Due to global warming and the toxins and greenhouse gasses in the air, people are becoming more sick and having respiratory issues.
                The forests around the world are burning, and since 1984, 23.5 million acres of forests have burned down in just the west in the United States.
                </p>
                <img src="../assets/images/First_Flowering_Index.gif">
                <p>	
                Plants have also started blooming earlier in the year. 
                This could have very negative side effects for numerous reasons. 
                One reason is because farmers could lose their crops.
                If the crops bloom early and then overnight get hit by a frost, the farmer could possibly lose a harvest. Another reason is animals are still in hibernation, and animals that are herbivores could lose their food. 
                </p>
        </div>
        <div class="global-api">
            <h2>The Current Carbon Intensity in England</h2>
        <CarbonIntensity />
        </div>
      <br><br> 
      
       <h3>Attributions</h3>
        <div class="attributions">
            <ul>
                <li>- UK plants flowering a month earlier due to climate change. University of Cambridge. (2022, February 2). Retrieved April 8, 2022, from https://www.cam.ac.uk/research/news/uk-plants-flowering-a-month-earlier-due-to-climate-change#:~:text=They%20found%20that%20the%20average,of%20the%20Royal%20Society%20B </li>
               <li>- Cook, J. (2010, April 13). Climate science glossary. Skeptical Science. Retrieved April 8, 2022, from https://skepticalscience.com/Flowers-blooming-earlier-now-than-any-time-in-last-250-years.html </li> 
                <li>- Brahic, C. (2007, May 16). Climate myths: The cooling after 1940 shows co2 does not cause warming. New Scientist. Retrieved April 8, 2022, from https://www.newscientist.com/article/dn11639-climate-myths-the-cooling-after-1940-shows-co2-does-not-cause-warming/ </li>
           
            </ul>




        </div>
        <TheFooter />

        
    </div>

</template>
<script setup>



</script>

<style scoped>
    .environment-body {
        padding: 1rem;
        text-align: center;
    }
    .global-api{
        text-align: center;
    }
    h1 {
    font-size:25px;
    text-align: center;
}
h2 {

font-size: 20px;

}

h3 {
    font-size:18px;
    text-align: center;
}
p {
    text-align: center;
    max-width:65ch;
    margin: 0 auto;
}
img {
    width:65%;
    margin-left: auto;
    margin-right: auto;
}
.attributions{

text-align: center;

}
</style>