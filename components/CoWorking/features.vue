<template>
  <div class="features">
    <div class="container features-body col ">
      <div class="features-header justify-content-between align-items-center">
        <div>
          <span class="features-span">FEATURES &nbsp;<img src="@/assets/img/events-marker.svg"
              alt="event marker"></span>
          <h2>Some General Info About<br /> Café One Features</h2>
        </div>
        <span class="features-text">
          Some info about each feature comes here and changes<br /> as the slider moves to each feature. The picture
          changes<br /> too
        </span>
      </div>
      <div class="tables">
        <div class="container col position-relative pl-0 pr-0">
          <div id="scene">
            <div id="middle-border"></div>
            <div id="left-zone">
              <ul class="list">
                <li class="item"><input type="radio" id="cozy-cafe" name="basic_carousel" value="cozy-cafe"
                    checked="checked" /><label class="label_feature" for="cozy-cafe">Cozy café</label>
                  <div class="content content_cozy-cafe"><span class="picto col-md-12"></span>

                  </div>
                </li>
                <li class="item"><input type="radio" id="radio_parking-area" name="basic_carousel"
                    value="parking-area" /><label class="label_feature" for="radio_parking-area">Spacious parking
                    area</label>
                  <div class="content content_parking-area"><span class="picto col-md-12"></span>

                  </div>
                </li>
                <li class="item"><input type="radio" id="radio_com-spaces" name="basic_carousel"
                    value="com-spaces" /><label class="label_feature" for="radio_com-spaces">Comfortable
                    spaces</label>
                  <div class="content content_com-spaces"><span class="picto col-md-12"></span>

                  </div>
                </li>
                <li class="item"><input type="radio" id="radio_playground" name="basic_carousel"
                    value="playground" /><label class="label_feature" for="radio_playground">Child playground</label>
                  <div class="content content_playground"><span class="picto col-md-12"></span>

                  </div>
                </li>
                <li class="item"><input type="radio" id="radio_outdoor" name="basic_carousel" value="outdoor" /><label
                    class="label_feature" for="radio_outdoor">Outdoor spaces</label>
                  <div class="content content_outdoor"><span class="picto col-md-12"></span>

                  </div>
                </li>
              </ul>
            </div>
            <div id="right-zone"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    name: "features",
  };

</script>
<style lang="scss" scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  .features-text {
    font-size: 20px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.46;
    letter-spacing: normal;
    color: #9A9A9A;
    text-align: start;
    font-family: Lato;
    margin-left: 0;
  }

  .features {
    margin: 40px 0px 0;
  }

  .features-body {
    width: 1150px;
    margin: auto;
    padding-top: 50px;
    padding-bottom: 20px;
  }

  .features-body h2 {
    font-size: 40px;
    font-weight: 800;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.18;
    letter-spacing: normal;
    color: #474E59;
    text-align: start;
    font-family: Lora;
  }

  .tables {
    border-radius: 2px;
    margin-bottom: 20px;
  }

  @media only screen and (max-width: 1150px) {
    .features-body {
      display: block;
      align-items: center;
      justify-content: center;
    }

    .features-body h2 {
      font-size: 32px;
    }

    .tables {
      width: 100%;
      height: auto;
      border-radius: 2px;
      background-color: #ffffff;
      margin-bottom: 20px;
      display: inline-block;
      align-items: center;
      justify-content: center;
      margin-top: 4rem;
    }

  }

  @media only screen and (max-width: 1150px) {
    .features-body {
      width: 99%;
    }
  }

  .features-header {
    display: block;
    padding-bottom: 3rem;

    @include breakpoint-min (md) {
      display: flex;
    }
  }

  .bg-black {
    background-color: #010101;
  }

  .text-red {
    color: #BC2934;
  }

  .features-type {
    font-family: Lato;
    font-style: normal;
    font-weight: bold;
    font-size: 20px;
    line-height: 24px;
    color: #222831;
    padding-left: 1rem;
    padding-top: 1rem;
  }

  .features-feature {
    font-family: Lato;
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 18px;
    color: #9A9A9A;
    padding-left: 1rem;
  }

  .features-span {
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 30px;
    color: #222831;
    margin: 0rem;
    font-family: Lato;
  }

  @keyframes slidein {
    0% {
      top: -400px;
      opacity: 0;
    }

    100% {
      opacity: 1;
      top: 0px;
    }
  }

  @keyframes slideout {
    0% {
      top: 0;
      opacity: 1;
    }

    100% {
      top: -400px;
      opacity: 0;
    }
  }

  #scene {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 400px;
    position: relative;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    margin: auto;
    overflow: hidden;
  }

  #scene #left-zone {
    background: #fff;
    height: 75%;
    flex-grow: 0;
    display: flex;
    width: 18.75rem;
    align-items: center;
    justify-content: flex-start;
  }

  #scene #left-zone .list {
    display: flex;
    list-style: none;
    align-content: stretch;
    flex-direction: column;
    flex-grow: 1;
    margin: 0;
    padding: 0;
  }

  #scene #left-zone .list li.item input[type="radio"] {
    display: none;
  }

  #scene #left-zone .list li.item input[type="radio"]~label {
    display: block;
    height: 50px;
    text-align: center;
    line-height: 50px;
  }

  #scene #left-zone .list li.item input[type="radio"]~label:first-letter {
    text-transform: uppercase;
  }

  #scene #left-zone .list li.item input[type="radio"]~label:hover {
    opacity: 0.5;
    cursor: pointer;
  }

  #scene #left-zone .list li.item input[type="radio"]~.content {
    position: absolute;
    left: 21.875rem;
    top: -25rem;
    width: 100%;
    height: 25rem;
    animation-duration: 0.75s;
    animation-name: slideout;
    animation-timing-function: ease-out;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
  }

  #scene #left-zone .list li.item input[type="radio"]~.content.content_cozy-cafe .picto {
    height: 100%;
    width: 100%;
    background-image: url('@/assets/img/gallery/gallery-4.jpeg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
  }

  #scene #left-zone .list li.item input[type="radio"]~.content.content_parking-area .picto {
    height: 100%;
    width: 100%;
    background-image: url('@/assets/img/gallery/gallery-10.jpeg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
  }

  #scene #left-zone .list li.item input[type="radio"]~.content.content_com-spaces .picto {
    height: 100%;
    width: 100%;
    background-image: url('@/assets/img/gallery/gallery-3.jpeg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
  }

  #scene #left-zone .list li.item input[type="radio"]~.content.content_playground .picto {
    height: 90%;
    width: 100%;
    background-image: url('@/assets/img/gallery/gallery-2.jpeg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
  }

  #scene #left-zone .list li.item input[type="radio"]~.content.content_outdoor .picto {
    height: 90%;
    width: 100%;
    background-image: url('@/assets/img/gallery/gallery-7.jpeg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
  }

  #scene #left-zone .list li.item input[type="radio"]~.content h1:first-letter {
    text-transform: uppercase;
  }

  #scene #left-zone .list li.item input[type="radio"]~.content p {
    max-width: 50%;
    text-align: center;
  }

  #scene #left-zone .list li.item input[type="radio"]:checked~label {
    opacity: 1;
    animation: all 1s cubic-bezier(0.455, 0.03, 0.515, 0.955);
  }

  label.label_feature {
    color: #222831;
  }

  #scene #left-zone .list li.item input[type="radio"]:checked~label.label_feature {
    border-left: solid 4px red;
    background: #BC2934;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
    color: #FFFFFF;
  }

  #scene #left-zone .list li.item input[type="radio"]:checked~.content {
    animation-duration: 0.75s;
    animation-name: slidein;
    animation-fill-mode: forwards;
    animation-timing-function: cubic-bezier(0.455, 0.03, 0.515, 0.955);
  }

  #scene #middle-border {
    background-color: #eee;
    height: 70%;
    flex-grow: 1;
    max-width: 2px;
    z-index: 0;
  }

  #scene #right-zone {
    background: #fff;
    height: 100%;
    flex-grow: 3;
    // @include breakpoint-max (md) {
    //   display: block;
    // }
  }

</style>
