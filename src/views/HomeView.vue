<template>
  <main>
    <section class="jumbotron">
      <div class="jumbotron-text">
        <h4>We are The Best</h4>
        <h1>
          Learn From Home With <span>The Best</span> Online Languange Tutors
        </h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id interdum
          dui mollis . Suspendisse nulla :
        </p>
        <button>Try Free Lesson</button>
      </div>
      <div class="jumbotron-image">
        <img src="../assets/new/hero-image.png" alt="hero" />
      </div>
    </section>
  </main>
</template>

<script setup></script>

<style lang="scss" scoped>
.jumbotron {
  display: flex;
  flex-direction: column;
  margin-top: 35px;

  h4 {
    position: relative;
    color: #fb9c46;
    font-size: 16px;
    font-weight: 600;
    display: inline-block;
    z-index: -1;

    &::after {
      content: '';
      position: absolute;
      right: -100px;
      top: 50%;
      width: 85px;
      height: 2px;
      background-color: #ff922f;
    }
  }

  h1 {
    margin-top: 15px;
    color: #000;
    font-size: 32px;
    font-weight: 700;
    line-height: 160%;
    letter-spacing: 1.12px;

    span {
      color: #fb9c46;
      font-weight: 700;
    }
  }

  p {
    margin-top: 15px;
    color: #90a3b4;
    font-weight: 400;
    line-height: 200%;
  }

  button {
    margin-top: 15px;
    padding: 15px 30px;
    background-color: #058e6e;
    border: none;
    border-radius: 16px;
    color: #fff;
    font-size: 18px;
    font-weight: 600;
    transition: 0.2s;

    &:hover {
      background-color: #2d6440;
    }
  }

  .jumbotron-image {
    margin-top: 65px;

    img {
      height: 315px;
    }
  }
}

@media (min-width: 768px) {
  .jumbotron {
    flex-direction: row;

    .jumbotron-image {
      flex: 1;

      img {
        width: 100%;
        height: auto;
      }
    }

    .jumbotron-text {
      flex: 1;
    }

    h1 {
      font-size: 48px;
    }
  }
}
</style>
