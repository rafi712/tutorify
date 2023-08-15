<template>
  <main>
    <section class="hero">
      <div class="hero-text">
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
      <div class="hero-image">
        <img src="@/assets/images/hero-image2.png" alt="hero" />
      </div>
    </section>

    <section class="offer">
      <div class="offer-text">
        <h4>What do you want to learn ?</h4>
        <h1>What We Offer</h1>
        <h4 class="lined">I want to learn</h4>
      </div>
      <div class="offer-contents">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec urna
          nec faucibus ridiculus placerat ipsum. Volutpat eget ut vitae amet
          ullamcorper et, ante venenatis.
        </p>
        <div class="items">
          <img src="@/assets/images/france.png" alt="france" />
          <img src="@/assets/images/germany.png" alt="germany" />
          <img src="@/assets/images/italia.png" alt="italia" />
          <img src="@/assets/images/japan.png" alt="japan" />
          <img src="@/assets/images/china.png" alt="china" />
          <img src="@/assets/images/russia.png" alt="russia" />
          <img src="@/assets/images/spain.png" alt="spain" />
          <div class="view-all">
            <p>View All</p>
            <img src="../assets/icons/arrow-down.svg" alt="arrow-down" />
          </div>
        </div>
      </div>
    </section>

    <section class="book">
      <div class="book-text">
        <h2>Purchase your awesome lessons and find your tutors</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Lorem
          habitant a tincidunt cras accumsan integer suscipit. Libero accumsan
          eget aliquet.
        </p>
        <div class="book-buttons">
          <button class="book-lessons-btn">Book Your Lessons</button>
          <button class="tutor-btn">Find Your Tutors</button>
        </div>
      </div>
      <div class="book-image">
        <img src="@/assets/images/Group.png" alt="" />
      </div>
    </section>
  </main>
</template>

<script setup></script>

<style lang="scss" scoped>
// Hero section start ================
.hero {
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
      height: 1px;
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
    box-shadow: 0px 4px 4px 0px rgba(64, 127, 85, 0.03),
      0px 10px 10px 0px rgba(64, 127, 85, 0.04),
      0px 25px 24px 0px rgba(64, 127, 85, 0.05),
      0px 85px 80px 0px rgba(64, 127, 85, 0.08);
    border: none;
    border-radius: 16px;
    color: #fff;
    font-size: 18px;
    font-weight: 600;
    transition: 0.2s;

    &:hover {
      background-color: #058063;
    }
  }

  .hero-image {
    margin-top: 65px;

    img {
      height: 315px;
    }
  }
}

@media (min-width: 768px) {
  .hero {
    flex-direction: row;

    .hero-image {
      flex: 1;

      img {
        width: 100%;
        height: auto;
      }
    }

    .hero-text {
      flex: 1;
    }

    h1 {
      font-size: 48px;
    }

    p {
      font-size: 16px;
      line-height: 180%;
    }
  }
}

// Hero section end ====================

// Offer section start =================
.offer {
  display: flex;
  flex-direction: column;
  margin: 68px 0;

  h4 {
    color: #fb9c46;
    font-size: 16px;
    font-weight: 600;

    &.lined {
      position: relative;
      display: inline-block;
      z-index: -1;

      &::after {
        content: '';
        position: absolute;
        right: -100px;
        top: 50%;
        width: 92px;
        height: 1px;
        background-color: #ff922f;
      }
    }
  }

  h1 {
    color: #393939;
    font-size: 30px;
    font-weight: 600;
    line-height: 160%; /* 48px */
    letter-spacing: 1.05px;
  }

  p {
    margin-top: 15px;
    color: #90a3b4;
    font-weight: 400;
    line-height: 200%;
  }

  .offer-contents {
    .items {
      margin-top: 40px;
      display: flex;
      gap: 35px;
      flex-wrap: wrap;

      img {
        height: 45px;
        width: 45px;
        filter: drop-shadow(0px -0.25px 3px rgba(0, 0, 0, 0.05))
          drop-shadow(0px -0.6px 8px rgba(0, 0, 0, 0.08))
          drop-shadow(0px -1px 16px rgba(0, 0, 0, 0.09))
          drop-shadow(0px -2.5px 32.5px rgba(0, 0, 0, 0.12))
          drop-shadow(0px -7px 89px rgba(0, 0, 0, 0.17));
      }

      .view-all {
        display: flex;
        align-items: center;
        cursor: pointer;

        p {
          color: #fb9c46;
          font-size: 18px;
          position: relative;
          top: -6px;
        }

        img {
          width: 25px;
          height: 25px;
        }
      }
    }
  }
}

@media (min-width: 768px) {
  .offer {
    flex-direction: row;
    // gap: 40px;

    .offer-text {
      flex: 1.3;

      h1 {
        font-size: 48px;
      }
    }

    .offer-contents {
      flex: 2;

      .items {
        margin-top: 20px;

        img {
          transition: 0.3s;

          &:hover {
            transform: scale(1.1);
          }
        }
      }
    }
  }
}
// Offer section end ===================

// Book section start ==================
.book {
  display: flex;
  flex-direction: column;
  align-items: center;

  .book-text {
    h2 {
      font-size: 30px;
      font-weight: 600;
      line-height: 160%; /* 57.6px */
      letter-spacing: 1.26px;
    }

    p {
      margin-top: 23px;
      color: #90a3b4;
      font-size: 12px;
      line-height: 200%; /* 24px */
    }

    .book-buttons {
      display: flex;
      justify-content: space-between;
      margin-top: 20px;

      button {
        width: 153px;
        height: 47px;
        border-radius: 16px;
        padding: 10px 16px;
        font-size: 12px;
        font-weight: 600;
      }

      .book-lessons-btn {
        border: none;
        background-color: #fb9c46;
        color: #fff;
      }

      .tutor-btn {
        border: 3px #fb9c46 solid;
        background-color: white;
        color: #fb9c46;
      }
    }
  }

  .book-image {
    img {
      width: 100%;
    }
  }
}

@media (min-width: 768px) {
  .book {
    flex-direction: row;

    .book-text {
      h2 {
        font-size: 36px;
      }

      p {
        font-size: 16px;
        line-height: 180%;
      }

      .book-buttons {
        justify-content: start;
        gap: 38px;

        button {
          width: 199px;
          height: 61px;
          font-size: 16px;
        }
      }
    }

    .book-image {
      img {
        width: 497px;
      }
    }
  }
}
// Book section end ====================
</style>
