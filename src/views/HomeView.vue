<template>
  <section id="home">
      <article class="flex_home article-color-main">
          <div id="div_p">
              
          </div>
      </article>
  </section>
</template>

<script setup>


onMounted(() => {
  let article_img = document.querySelector('.../public./Images/home.png');

  gsap.fromTo(article_img, {
      opacity: 0,
      x: '-100%',
  }, {
      opacity: 1,
      x: 0,
      duration: 1,
      delay: 1
  });
  gsap.fromTo('.article_p', {
      opacity: 0,
      x: '100%',
      delay: 2
  }, {
      opacity: 1,
      x: 0,
      duration: 1,
      delay: 2,
      stagger: .5
  })
})
</script>

<style lang="scss" scoped>
#div_p{
  display: flex;
  flex-direction: column;
  gap: 30px;
}

img{
  opacity: 0;
  width: 20rem;
  height: 20rem;
  border-radius: 50%;
  box-shadow: 2px 5px 10px black;
}

p{
  font-weight: 300;
  width: 30rem;
  text-align: justify;
  line-height: 1.3;
}
</style>