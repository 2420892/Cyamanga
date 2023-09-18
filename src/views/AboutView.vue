<template>
  <div id="about" class="container">

    <div class="text">
      <h1>About Siyamanga</h1>
      <p>
        I am a 22 year old female from Mfuleni, Cape Town. I recently completed my software development course at Life Choices Academy, where I not only gained technical expertise but also delved into the world of professional development and acquired valuable life skills.</p>
    
      <p>  I've also had the privilege of developing my public speaking abilities during my time with the Department of Water and Sanitation (DWS). I've proudly served as a Constitution Reviewer for Metanoia Residence at Stellenbosch University.</p>
    
       <p>I consider myself an attentive, intuitive, and flexible learner with leadership skills. My strengths shine both in collaborative team environments and when I'm tackling tasks independently.</p> 
    
       <p> Having successfully completed my software development course, I'm now eagerly seeking internship or junior developer opportunities to apply and expand upon my knowledge and skills.</p>
    
       <p> Outside of my academic and professional pursuits, I have a passion for chorale music and often find solace in singing. Additionally, I find great fulfillment in contributing to my community. I've dedicated my time to volunteering at Masgcine Children's Home annd at Indaba zosindiso Soup Kitchen, where I've been able to make a positive impact and give back to those in need.
    </p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style  scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;

}

.text {
  width: 55rem;
  margin:18px;
  border: 1px solid #13292a;
  padding: 8px;
  box-shadow: 8px 16px 0px #13292a;
  border-radius: 12px;
  font-size: 25px;
}


@media (width < 570px) {
  .text {
    font-size: inherit;
    margin-top: 0px;
  }
}
</style>