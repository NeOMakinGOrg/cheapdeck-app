<template>
  <div class="grid">
    <ul class="grid-list">
      <li class="grid-item">
        <div class="grid-item-content">
          <img
            class="grid-item-image"
            src="../assets/disabled-microphone.webp"
          />
          <p class="grid-item-title">1 (F13)</p>
        </div>
      </li>
      <li class="grid-item">
        <div class="grid-item-content">
          <img
            class="grid-item-image"
            src="../assets/disabled-microphone.webp"
          />
          <p class="grid-item-title">2 (F14)</p>
        </div>
      </li>
      <li class="grid-item">
        <div class="grid-item-content">
          <img
            class="grid-item-image"
            src="../assets/disabled-microphone.webp"
          />
          <p class="grid-item-title">3 (F15)</p>
        </div>
      </li>
      <li class="grid-item grid-item-arrow-up">
        <div class="grid-item-content">
          <div class="grid-item-image">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
              version="1.1"
              id="Capa_1"
              x="0px"
              y="0px"
              width="960px"
              height="560px"
              viewBox="0 0 960 560"
              enable-background="new 0 0 960 560"
              xml:space="preserve"
            >
              <g id="Rounded_Rectangle_33_copy_4_1_">
                <path
                  d="M480,344.181L268.869,131.889c-15.756-15.859-41.3-15.859-57.054,0c-15.754,15.857-15.754,41.57,0,57.431l237.632,238.937   c8.395,8.451,19.562,12.254,30.553,11.698c10.993,0.556,22.159-3.247,30.555-11.698l237.631-238.937   c15.756-15.86,15.756-41.571,0-57.431s-41.299-15.859-57.051,0L480,344.181z"
                />
              </g>
            </svg>
          </div>
          <p class="grid-item-title">Up</p>
        </div>
      </li>
      <li class="grid-item">
        <div class="grid-item-content">
          <img
            class="grid-item-image"
            src="../assets/disabled-microphone.webp"
          />
          <p class="grid-item-title">4 (F16)</p>
        </div>
      </li>
      <li class="grid-item">
        <div class="grid-item-content">
          <img
            class="grid-item-image"
            src="../assets/disabled-microphone.webp"
          />
          <p class="grid-item-title">5 (f17)</p>
        </div>
      </li>
      <li class="grid-item">
        <div class="grid-item-content">
          <img
            class="grid-item-image"
            src="../assets/disabled-microphone.webp"
          />
          <p class="grid-item-title">6 (F18)</p>
        </div>
      </li>
      <li class="grid-item">
        <div class="grid-item-content">
          <div class="grid-item-image">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
              version="1.1"
              id="Capa_1"
              x="0px"
              y="0px"
              width="960px"
              height="560px"
              viewBox="0 0 960 560"
              enable-background="new 0 0 960 560"
              xml:space="preserve"
            >
              <g id="Rounded_Rectangle_33_copy_4_1_">
                <path
                  d="M480,344.181L268.869,131.889c-15.756-15.859-41.3-15.859-57.054,0c-15.754,15.857-15.754,41.57,0,57.431l237.632,238.937   c8.395,8.451,19.562,12.254,30.553,11.698c10.993,0.556,22.159-3.247,30.555-11.698l237.631-238.937   c15.756-15.86,15.756-41.571,0-57.431s-41.299-15.859-57.051,0L480,344.181z"
                />
              </g>
            </svg>
          </div>
          <p class="grid-item-title">Down</p>
        </div>
      </li>
    </ul>
    <p class="grid-page">Page: 1</p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Grid',
});
</script>

<style lang="scss">
.grid {
  &-item {
    list-style-type: none;

    &-content {
      width: 50px;
      height: 50px;
      background: rgba(255, 255, 255, 0.8);
      margin: 10px;
      display: block;
      position: relative;
      border-radius: 6px;
      box-shadow: 0 0 1rem 0 rgba(0, 0, 0, 0.8);
    }

    &-title {
      color: white;
      font-size: 10px;
      margin: 0;
      line-height: 10px;
      position: absolute;
      left: 5px;
      top: -15px;
    }
  }

  &-item {
    display: flex;
    align-items: center;
    justify-content: center;

    &-image {
      padding: 10px;
      max-width: calc(100% - 20px);
      max-height: calc(100% - 20px);
      display: flex;
      align-items: center;
      justify-content: center;

      svg {
        width: 100%;
      }
    }

    &-arrow-up {
      svg {
        transform: rotate(180deg);
      }
    }
  }

  &-list {
    max-width: 300px;
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    justify-content: space-around;
    margin: 0;
    padding: 0;
  }

  &-page {
    color: white;
    font-size: 10px;
    margin: 0;
    text-align: right;
    padding: 0 20px;
  }
}
</style>
