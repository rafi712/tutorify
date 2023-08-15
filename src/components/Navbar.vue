<template>
  <header>
    <nav>
      <p class="brand">Tutorify</p>
      <div class="desktop-menu">
        <a>Home</a>
        <a>Lesson</a>
        <a>Find Tutors</a>
        <a>About Us</a>

        <button class="login-btn">Login</button>
        <button class="signup-btn">Sign Up</button>
      </div>

      <div class="mobile-menu">
        <img
          v-if="isActive"
          src="@/assets/icons/ci_close.svg"
          alt="close"
          @click="toggleMenu"
        />
        <img
          v-else
          src="@/assets/icons/ci_hamburger.svg"
          alt="hamburger"
          @click="toggleMenu"
        />
        <Transition>
          <div class="dropdown" v-if="isActive">
            <a>Home</a>
            <a>Lesson</a>
            <a>Find Tutors</a>
            <a>About Us</a>

            <button class="login-btn">Login</button>
            <button class="signup-btn">Sign Up</button>
          </div>
        </Transition>
      </div>
    </nav>
    <hr />
  </header>
</template>

<script setup>
import { computed, ref } from 'vue'

const isActive = ref(false)

const toggleMenu = () => {
  isActive.value = !isActive.value
}

const toggleIcon = computed(() => {
  return isActive.value
    ? require('@/assets/icons/ci_close.svg')
    : require('@/assets/icons/ci_hamburger.svg')
})
</script>

<style lang="scss" scoped>
header {
  position: sticky;
  top: 0;
  z-index: 100;
  padding: 45px 25px 0;
  background-color: #fff;

  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 23px;

    .brand {
      font-size: 18px;
      color: #393939;
      font-weight: 700;
    }
  }

  hr {
    height: 1px;
    background-color: #c4c4c4;
  }
}

.desktop-menu {
  display: none;
  align-items: center;
  gap: 50px;

  a {
    font-weight: 600;
    transition: 0.2s;
    position: relative;

    &:hover {
      color: #ff922f;
    }

    &:hover::after {
      content: '';
      position: absolute;
      bottom: -1;
      left: 0;
      margin-top: 25px;
      background-color: #ff922f;
      border-radius: 5px;
      height: 3px;
      width: 100%;
    }
  }

  button {
    width: 102px;
  }
}

.mobile-menu {
  position: relative;

  img {
    cursor: pointer;
  }
}

.dropdown {
  min-width: 200px;
  padding: 15px;
  position: absolute;
  right: 0;
  top: 70;
  display: flex;
  flex-direction: column;
  gap: 7px;
  border: 1px #c4c4c4 solid;
  background-color: #fff;
  z-index: 10;
  border-radius: 8px;

  a {
    position: relative;
    font-weight: 600;
    transition: 0.2s;

    &:hover {
      color: #ff922f;
    }

    // &:hover::after {
    //   content: '';
    //   position: absolute;
    //   display: block;
    //   bottom: 0;
    //   left: 0;
    //   height: 2px;
    //   background-color: #ff922f;
    //   width: fit-content;
    // }
  }

  button:first-of-type {
    margin-top: 20px;
  }
}

button {
  padding: 10px 16px;
  border-radius: 8px;
  border: none;
  color: #fff;
  font-size: 16px;
  font-family: poppins;
  font-weight: 600;
}

.login-btn {
  background-color: #407f55;
  transition: 0.2s;

  &:hover {
    background-color: #2d6440;
  }
}

.signup-btn {
  background-color: #fb9c46;
  transition: 0.2s;

  &:hover {
    background-color: #dd822d;
  }
}

.v-enter-active,
.v-leave-active {
  transition: opacity 0.3s ease;
}

.v-enter-from,
.v-leave-to {
  opacity: 0;
}

@media (min-width: 768px) {
  .mobile-menu {
    display: none;
  }

  .desktop-menu {
    display: flex;
  }
}
</style>
