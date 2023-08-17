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
            <img src="@/assets/icons/arrow-down.svg" alt="arrow-down" />
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
        <img src="@/assets/images/book-section.png" alt="book-section" />
      </div>
    </section>

    <section class="benefit">
      <div class="benefit-content">
        <h2>What Will You <span>Get</span> ?</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id interdum
          dui mollis . Suspendisse nulla :
        </p>
        <div class="benefit-item">
          <img src="@/assets/icons/tick-green.svg" alt="tick" />
          <div class="description">
            <p>1-on-1 lessons in more than 150 languages</p>
            <p>
              <span>
                Learn from certified teachers with proven experience@.
                <span class="green">read more</span>
              </span>
            </p>
          </div>
        </div>
        <div class="benefit-item">
          <img src="@/assets/icons/tick-green.svg" alt="tick" />
          <div class="description">
            <p>Practice for free with the italki community</p>
            <p>
              <span>
                Develop your language skills by building connections with
                others@.
                <span class="green">read more</span>
              </span>
            </p>
          </div>
        </div>
        <div class="benefit-item">
          <img src="@/assets/icons/tick-green.svg" alt="tick" />
          <div class="description">
            <p>Take learning beyond the classroom</p>
            <p>
              <span>
                Learn from certified teachers with proven experience@.
                <span class="green">read more</span>
              </span>
            </p>
          </div>
        </div>
      </div>
      <div class="benefit-image">
        <img src="@/assets/images/benefit-section.png" alt="benefit-section" />
      </div>
    </section>

    <section class="how-it-works">
      <div class="how-it-works-content">
        <h2>Here's how it <span>works</span></h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Lorem
          habitant a tincidunt cras accumsan integer suscipit. Libero accumsan
          eget aliquet.
        </p>
        <div class="steps">
          <div class="step">
            <img src="@/assets/icons/user-steps.svg" alt="" />
            <div class="description">
              <p>Find a tutor</p>
              <p>
                Choose your ideal teacher from over 10,000 qualified language
                tutors.
              </p>
            </div>
          </div>
          <div class="step">
            <img src="@/assets/icons/user-steps.svg" alt="" />
            <div class="description">
              <p>Find a tutor</p>
              <p>
                Choose your ideal teacher from over 10,000 qualified language
                tutors.
              </p>
            </div>
          </div>
          <div class="step">
            <img src="@/assets/icons/user-steps.svg" alt="" />
            <div class="description">
              <p>Find a tutor</p>
              <p>
                Choose your ideal teacher from over 10,000 qualified language
                tutors.
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="how-it-works-image">
        <img src="@/assets/images/how-to-works-section.png" alt="" />
      </div>
    </section>
  </main>
</template>

<script setup></script>

<style lang="scss" scoped>
// Hero section start ==================
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
      font-size: 15px;
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

// Benefit section start ===============
.benefit {
  margin-top: 20px;
  .benefit-content {
    h2 {
      color: #393939;
      font-size: 30px;
      font-weight: 600;
      line-height: 160%;
      letter-spacing: 1.05px;

      span {
        color: #058e6e;
        font-size: inherit;
        font-weight: inherit;
        line-height: inherit;
        letter-spacing: inherit;
      }
    }

    p {
      margin-top: 5px;
      color: #90a3b4;
      font-size: 15px;
      line-height: 200%; /* 24px */
    }

    .benefit-item {
      margin-top: 30px;
      padding: 11px;
      display: flex;
      gap: 16px;
      align-items: start;
      border-radius: 16px;
      background: #fff;
      box-shadow: 0px -2px 128px 0px rgba(5, 142, 110, 0.14);

      p {
        color: #393939;
        font-size: 15px;
        font-weight: 600;
        line-height: 170%;

        &:nth-of-type(2) {
          display: list-item;
          color: #8d8d8d;
          font-size: 13px;
          font-weight: 400;
          line-height: 200%;
          position: relative;
          left: 11px;

          .green {
            color: #058e6e;
          }
        }
      }
    }
  }

  .benefit-image {
    margin-top: 40px;

    img {
      width: 100%;
    }
  }
}

@media (min-width: 768px) {
  .benefit {
    display: flex;
    flex-direction: row-reverse;
    gap: 86px;

    .benefit-content {
      flex: 1;

      h2 {
        font-size: 36px;
      }

      p {
        font-size: 16px;
        line-height: 180%; /* 28.8px */
      }

      .benefit-item {
        padding: 18px;

        img {
          width: 52px;
        }

        p {
          font-size: 16px;

          &:nth-of-type(2) {
            font-size: 15px;
            line-height: 160%; /* 22.4px */
          }
        }
      }
    }

    .benefit-image {
      flex: 1;
    }
  }
}
// Benefit section end =================

// How-it-works section start ==========
.how-it-works {
  margin-top: 65px;
  display: flex;
  flex-direction: column;
  gap: 56px;

  .how-it-works-content {
    h2 {
      color: #393939;
      font-size: 30px;
      font-weight: 600;
      line-height: 160%;
      letter-spacing: 1.05px;

      span {
        color: #fb9c46;
        font-size: inherit;
        font-weight: inherit;
        line-height: inherit;
        letter-spacing: inherit;
      }
    }

    p {
      margin-top: 15px;
      color: #90a3b4;
      font-size: 15px;
      line-height: 200%; /* 24px */
    }

    .steps {
      display: flex;
      flex-direction: column;
      gap: 20px;
      margin-top: 25px;

      p {
        margin-top: 0;
      }
      .step {
        display: flex;
        gap: 22px;
        align-items: start;
        padding: 14px;
        border-radius: 10px;
        background-color: #fff;
        box-shadow: 0px 0.5px 45px 0px rgba(255, 146, 47, 0.08),
          0px 4px 357px 0px rgba(255, 146, 47, 0.15);

        img {
          width: 35px;
          margin-top: 5px;
        }

        p {
          color: #fb9c46;
          font-size: 15px;
          line-height: 170%;

          &:nth-of-type(2) {
            font-size: 13px;
            color: #393939;
            line-height: 170%;
          }
        }
      }
    }
  }

  .how-it-works-image {
    img {
      width: 325px;
    }
  }
}

@media (min-width: 768px) {
  .how-it-works {
    flex-direction: row;
    gap: 100px;

    .how-it-works-content {
      flex: 1;

      h2 {
        font-size: 36px;
        letter-spacing: 1.26px;
      }

      p {
        font-size: 16px;
        line-height: 180%; /* 28.8px */
      }

      .steps {
        gap: 35px;

        .step {
          img {
            width: 40px;
          }

          p {
            font-size: 16px;

            &:nth-of-type(2) {
              font-size: 15px;
              line-height: 160%; /* 22.4px */
            }
          }
        }
      }
    }

    .how-it-works-image {
      flex: 1;

      img {
        width: 517px;
        margin-top: 75px;
      }
    }
  }
}
// How-it-works section end ============
</style>
