<template>
  <div>
    <div class="l-page js-pjax-page" data-page-id="index">
      <div class="l-dummy-scroll js-dummy-scroll"></div>
      <div class="l-global-parts">
        <h1 class="p-global-logo">
          <a class="js-global-logo" href="/">
            <img src="~assets/img/kb-logo.png" height="50px"/>
            <!-- <svg width="28" height="28" role="img" aria-labelledby="hassyadai-logo-title">
              <title id="hassyadai-logo-title">HASSYADAI ハッシャダイ</title>
              <path d="M27 28h-9v-9h-8v9H0V0h10v9h8V0h10v28h-1zM4 27h2v-2H4v2zm0-3h2v-2H4v2zm0-3h2v-2H4v2zm-3 6h2v-2H1v2zm0-3h2v-2H1v2zm0-3h2v-2H1v2zM9 1H1v2h8V1zm0 3H1v2h8V4zm0 3H1v2h8V7zm0 3H1v2h8v-2zm0 3H1v2h8v-2zm0 3H1v2h8v-2zm0 3H7v2h2v-2zm0 3H7v2h2v-2zm0 3H7v2h2v-2zm3-15h-2v2h2v-2zm0 3h-2v2h2v-2zm0 3h-2v2h2v-2zm3-6h-2v2h2v-2zm0 3h-2v2h2v-2zm0 3h-2v2h2v-2zm10 11h2v-2h-2v2zm0-3h2v-2h-2v2zm0-3h2v-2h-2v2zm-3 6h2v-2h-2v2zm0-3h2v-2h-2v2zm0-3h2v-2h-2v2zm-3 6h2v-2h-2v2zm0-3h2v-2h-2v2zm0-3h2v-2h-2v2zm-3-3h2v-2h-2v2zm0-3h2v-2h-2v2zm0-5v2h2v-2h-2zm3-9v17h2V1h-2zm3 0v17h2V1h-2zm3 0v17h2V1h-2z"></path>
            </svg> -->
          </a>
        </h1>
        <!-- <div class="p-global-category" id="vue-global-category">
          <div class="p-global-category__label u-tt-u" :key="key" v-for="(item, key) in items" v-html="item.content" :class="{ 'is-shown' : key === currentKey, 'is-hidden' : key !== currentKey }"></div>
          <div class="p-global-category__bg" :style="setLabelStyle"></div>
        </div> -->
        <!-- <div class="p-global-share">
          <div class="p-global-share__sns">
            <a class="p-global-share__sns-item" href="https://www.facebook.com/hassyadai/" target="_blank">
              <svg class="c-icon-facebook" xmlns="http://www.w3.org/2000/svg" role="img" aria-labelledby="icon-facebook-title" width="7" height="14" viewBox="0 0 117.7 226.6" id="icon-facebook">
                <title id="icon-facebook-title">Facebook</title>
                <path d="M76.4 226.6V123.2h34.7l5.2-40.3H76.4V57.2c0-11.7 3.2-19.6 20-19.6h21.3v-36C114 1.1 101.3 0 86.6 0 55.8 0 34.8 18.8 34.8 53.2v29.7H0v40.3h34.8v103.4h41.6z"></path>
              </svg>
            </a>
            <a class="p-global-share__sns-item" href="https://twitter.com/hassyadai" target="_blank">
              <svg class="c-icon-twitter" xmlns="http://www.w3.org/2000/svg" role="img" aria-labelledby="icon-twitter-title" width="15" height="13" viewBox="0 0 273.4 222.2" id="icon-twitter">
                <title id="icon-twitter-title">Twitter</title>
                <path d="M273.4 26.3c-10.1 4.5-20.9 7.5-32.2 8.8 11.6-6.9 20.5-17.9 24.7-31-10.9 6.4-22.9 11.1-35.7 13.6C220 6.8 205.4 0 189.3 0c-31 0-56.1 25.1-56.1 56.1 0 4.4.5 8.7 1.5 12.8C88 66.5 46.7 44.2 19 10.3c-4.8 8.3-7.6 17.9-7.6 28.2 0 19.5 9.9 36.6 25 46.7-9.2-.3-17.8-2.8-25.4-7v.7c0 27.2 19.3 49.8 45 55-4.7 1.3-9.7 2-14.8 2-3.6 0-7.1-.4-10.6-1 7.1 22.3 27.9 38.5 52.4 39-19.2 15-43.4 24-69.7 24-4.5 0-9-.3-13.4-.8 24.8 15.9 54.3 25.2 86 25.2 103.2 0 159.6-85.5 159.6-159.6 0-2.4-.1-4.9-.2-7.3 11.1-8 20.6-17.9 28.1-29.1z"></path>
              </svg>
            </a>
            <a class="p-global-share__sns-item" href="https://www.instagram.com/hassyadai/" target="_blank">
              <svg class="c-icon-instagram" xmlns="http://www.w3.org/2000/svg" role="img" aria-labelledby="icon-instagram-title" width="14" height="14" viewBox="0 0 24 24" id="icon-instagram">
                <title id="icon-instagram-title">Instagram</title>
                <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"></path>
              </svg>
            </a>
            <a class="p-global-share__sns-item" href="https://line.me/R/ti/p/%40uvi1849z" target="_blank">
              <svg class="c-icon-line-at" xmlns="http://www.w3.org/2000/svg" role="img" aria-labelledby="icon-line-at-title" width="14" height="14" viewBox="0 0 14 14" id="icon-line-at">
                <title id="icon-line-at-title">Line@</title>
                <path d="M7 .1C3.2.1.1 3.2.1 7s3.1 6.9 6.9 6.9c.7 0 1.4-.1 2.1-.3l.4-.1c.1 0 .2-.2.2-.3L9.3 12c0-.1-.2-.2-.3-.2l-.4.1c-.5.2-1 .2-1.6.2-2.8 0-5.1-2.3-5.1-5.1S4.2 1.9 7 1.9s5.1 2.3 5.1 5.1c0 .6-.1 1.2-.3 1.8-.2.4-.5.8-.8.8-.4 0-.7-.3-.7-.7V4c0-.2-.1-.3-.3-.3H8.7c-.2 0-.3.1-.3.3v.1L8.3 4c-.5-.3-1-.4-1.6-.4-1.8 0-3.3 1.5-3.3 3.4s1.5 3.4 3.4 3.4c.6 0 1.3-.2 1.8-.5h.1v.1c.4.9 1.3 1.5 2.3 1.5 1.1 0 2.1-.8 2.5-2 .3-.8.4-1.6.4-2.4 0-3.9-3.1-7-6.9-7zM8.4 7c0 .9-.7 1.7-1.7 1.7S5.1 7.9 5.1 7s.7-1.7 1.7-1.7 1.6.8 1.6 1.7z"></path>
              </svg>
            </a>
          </div>
          <div class="p-global-share__line"></div>
          <div class="p-global-share__label">Be Collective For Customer Delight</div>
        </div>
        <div class="p-global-contact">
          <a class="p-global-contact__item" href="https://chatform.me/hassyadai" target="_blank">
            <div class="c-link-rect">
              <div class="c-link-rect__label">企業・保護者・採用</div>
            </div>
            <img class="p-global-contact__handshake" src="/img/pc/common/icon_handshake.png" alt="">
          </a>
          <a class="p-global-contact__item" href="https://hassyadai.com/ctbt" target="_blank">
            <div class="c-link-rect">
              <div class="c-link-rect__label">若者はこちら</div>
            </div>
            <img class="p-global-contact__rocket" src="/img/pc/common/icon_rocket.png" alt="">
          </a>
          <div class="p-global-contact-dialog" id="vue-contact-dialog" :class="{ 'is-shown' : state === 1, 'is-hidden' : state === 2 }">
            <div class="p-global-contact-dialog__text">ヤンキーインターンに<br>参加の方はこちらから！</div>
            <div class="p-global-contact-dialog__close" @click="hide"></div>
          </div>
        </div> -->
        <div id="vue-global-navi">
          <div class="p-hamburger is-valid" :class="{ 'is-opened-navi' : isOpenedNavi === 1, 'is-expand' : isExpand, 'is-over' : isOveredHamburger === 1, 'is-leave' : isOveredHamburger === 2 }" @click="toggleNavi" @mouseover="mouseoverHamburger" @mouseout="mouseoutHamburger">
            <div class="p-hamburger__line p-hamburger__line--01">
              <div class="p-hamburger__line-in p-hamburger__line-in--01"></div>
            </div>
            <div class="p-hamburger__line p-hamburger__line--02">
              <div class="p-hamburger__line-in p-hamburger__line-in--02"></div>
            </div>
            <div class="p-hamburger__line p-hamburger__line--cross01">
              <div class="p-hamburger__line-in p-hamburger__line-in--cross01"></div>
            </div>
            <div class="p-hamburger__line p-hamburger__line--cross02">
              <div class="p-hamburger__line-in p-hamburger__line-in--cross02"></div>
            </div>
          </div>
          <div class="p-gnav" :class="{ 'is-opened' : isOpenedNavi === 1, 'is-closed' : isOpenedNavi === 2 }">
            <div class="p-gnav__wrap">
              <div class="p-gnav__main">
                <a class="p-gnav-main-item u-tt-u js-hover js-cc-link" href="/" :class="{ 'is-disabled' : isCurrentId === 1 }">
                  <div class="p-gnav-main-item__num">.01</div>
                  <div class="p-gnav-main-item__line"></div>
                  <div class="p-gnav-main-item__label">Home</div>
                </a>
                <a class="p-gnav-main-item u-tt-u js-hover js-cc-link" href="#about" :class="{ 'is-disabled' : isCurrentId === 2 }">
                  <div class="p-gnav-main-item__num">.02</div>
                  <div class="p-gnav-main-item__line"></div>
                  <div class="p-gnav-main-item__label">About</div>
                </a>
                <a class="p-gnav-main-item u-tt-u js-hover js-cc-link" href="#portfolio" :class="{ 'is-disabled' : isCurrentId === 3 }">
                  <div class="p-gnav-main-item__num">.03</div>
                  <div class="p-gnav-main-item__line"></div>
                  <div class="p-gnav-main-item__label">Portfolio</div>
                </a>
                <a class="p-gnav-main-item u-tt-u js-hover js-cc-link" href="#resume" :class="{ 'is-disabled' : isCurrentId === 4 }">
                  <div class="p-gnav-main-item__num">.04</div>
                  <div class="p-gnav-main-item__line"></div>
                  <div class="p-gnav-main-item__label">Resume</div>
                </a>
                <a class="p-gnav-main-item u-tt-u js-hover js-cc-link" href="#contact" :class="{ 'is-disabled' : isCurrentId === 5 }">
                  <div class="p-gnav-main-item__num">.05</div>
                  <div class="p-gnav-main-item__line"></div>
                  <div class="p-gnav-main-item__label">Contact</div>
                </a>
              </div>
              <!-- <div class="p-gnav__sub"><a class="p-gnav-sub-item u-tt-u js-hover js-cc-link" href="/company/" :class="{ 'is-disabled' : isCurrentId === 10 }">Company</a><a class="p-gnav-sub-item u-tt-u js-hover js-cc-link" href="https://www.wantedly.com/companies/hassyadai?ql=gaJpZM4AROMS" target="_blank"  >Recruit</a><a class="p-gnav-sub-item u-tt-u js-hover js-cc-link" href="/privacypolicy/" :class="{ 'is-disabled' : isCurrentId === 11 }">Privacy Policy</a></div> -->
            </div>
            <!-- <div class="p-gnav__copyright">HASSYADAI.com Copyright 2018</div> -->
          </div>
        </div>
        <div class="p-progress-circle" :class="{ 'is-opened-gnav' : isOpenedNavi === 1 }">
          <div class="p-progress-circle__label"></div>
          <canvas class="p-progress-circle__canvas" id="progress-circle" width="50" height="50"></canvas>
        </div>
      </div>
      <div class="l-contents js-contents js-pjax-contents" :class="{ 'is-opened-gnav' : isOpenedNavi === 1, 'is-arrived is-fixed' : isOpenedNavi === 2 }">
        <div class="p-index-scene">
          <div class="p-index-section p-index-kv vue-choose-your-life">
            <!-- <div class="p-intern-category-kv__category-label u-tt-u">
              <div class="p-intern-category-kv__category-label-in">Front-End Developer</div>
            </div> -->
            <h1 class="p-intern-category-kv__head c-heading-huge">
              <div class="c-perspective u-tt-u">
                <span class="c-noise-str c-noise-str--4 js-noise-str">k</span>
                <span class="c-noise-str c-noise-str--1 js-noise-str">e</span>
                <span class="c-noise-str c-noise-str--3 js-noise-str">a</span>
                <span class="c-noise-str c-noise-str--3 js-noise-str">n</span>
                <span class="c-noise-str c-noise-str--2 js-noise-str">n</span>
              </div>
            </h1>
            <!-- <div class="p-index-section__in">
              <div class="p-index-kv__slogan c-perspective" :class="{ 'lid' : isValid === true, 'is-shown' : focusId &lt; 0, 'is-hidden' : focusId &gt; -1 }">
                <div class="p-index-kv__slogan-in"><img src="/img/pc/index/kv_slogan.svg" alt="Choose Your Life"></div>
              </div>
              <div class="p-person p-person--business p-person p-person--business-side" :class="{ 'is-focus' : focusId === 0, 'is-not-focus' : focusId === 1 }"><img src="~assets/img/pc/common/bg_business.png" alt=""></div>
              <div class="p-person p-person--hacker p-person p-person--hacker-side" :class="{ 'is-focus' : focusId === 1, 'is-not-focus' : focusId === 0 }"><img src="~assets/img/pc/common/bg_hacker.png" alt=""></div>
            </div>
            <a class="p-index-kv__link p-index-kv__link--business" href="/yankee_intern/business/" @mouseover="mouseover(0)" @mouseleave="mouseleave" @click="choose" :class="{ 'is-disabled' : isValid === false }">Business</a><a class="p-index-kv__link p-index-kv__link--hacker" href="/yankee_intern/hacker/" @mouseover="mouseover(1)" @mouseleave="mouseleave" @click="choose" :class="{ 'is-disabled' : isValid === false }">Hacker</a>
            <div class="p-index-kv__label" :class="{ 'is-shown' : focusId === 0, 'is-hidden' : focusId !== 0 }">
              <div class="c-heading-huge c-perspective u-tt-u"><span class="c-noise-str c-noise-str--4 js-noise-str">B</span><span class="c-noise-str c-noise-str--1 js-noise-str">u</span><span class="c-noise-str c-noise-str--3 js-noise-str">s</span><span class="c-noise-str c-noise-str--3 js-noise-str">i</span><span class="c-noise-str c-noise-str--2 js-noise-str">n</span><span class="c-noise-str c-noise-str--3 js-noise-str">e</span><span class="c-noise-str c-noise-str--2 js-noise-str">s</span><span class="c-noise-str c-noise-str--3 js-noise-str">s</span>
              </div>
            </div>
            <div class="p-index-kv__label" :class="{ 'is-shown' : focusId === 1, 'is-hidden' : focusId !== 1 }">
              <div class="c-heading-huge c-perspective u-tt-u"><span class="c-noise-str c-noise-str--4 js-noise-str">H</span><span class="c-noise-str c-noise-str--1 js-noise-str">a</span><span class="c-noise-str c-noise-str--3 js-noise-str">c</span><span class="c-noise-str c-noise-str--3 js-noise-str">k</span><span class="c-noise-str c-noise-str--2 js-noise-str">e</span><span class="c-noise-str c-noise-str--3 js-noise-str">r</span>
              </div>
            </div> -->
          </div>
          <div class="p-index-section">
            <div class="p-index-section__in p-index-pride">
              <h2 class="p-index-pride__head">
                <div class="c-perspective u-tt-u">
                  <span class="c-noise-str c-noise-str--4 js-noise-str">A</span>
                  <span class="c-noise-str c-noise-str--1 js-noise-str">b</span>
                  <span class="c-noise-str c-noise-str--3 js-noise-str">o</span>
                  <span class="c-noise-str c-noise-str--3 js-noise-str">u</span>
                  <span class="c-noise-str c-noise-str--2 js-noise-str">t</span>
                </div>
              </h2>
              <p class="p-index-pride__excerpt c-transit-fade">Lorem ipsum dolor sit amet consectetur <br> adipisicing elit. <br>Nemo consequatur dicta sapiente cumque ad <br>aspernatur necessitatibus vero? Enim recusandae quod <br>porro omnis eligendi fugiat blanditiis,<br> eveniet deserunt in excepturi nobis.</p>
              <div class="p-index-pride__link c-transit-fade u-tt-u">
                <a class="c-link-rect" href="/">
                  <div class="c-link-rect__label">About Me</div>
                </a>
              </div>
            </div>
          </div>
          <div class="p-index-section">
            <div class="p-index-section__in p-index-has-figure">
              <h2 class="p-index-has-figure__head">
                <div class="c-perspective u-tt-u">
                  <span class="c-noise-str c-noise-str--4 js-noise-str">P</span>
                  <span class="c-noise-str c-noise-str--1 js-noise-str">o</span>
                  <span class="c-noise-str c-noise-str--3 js-noise-str">r</span>
                  <span class="c-noise-str c-noise-str--3 js-noise-str">t</span>
                  <span class="c-noise-str c-noise-str--2 js-noise-str">f</span>
                  <span class="c-noise-str c-noise-str--3 js-noise-str">o</span>
                  <span class="c-noise-str c-noise-str--2 js-noise-str">l</span>
                  <span class="c-noise-str c-noise-str--1 js-noise-str">i</span>
                  <span class="c-noise-str c-noise-str--4 js-noise-str">o</span>
                </div>
              </h2>
              <div class="p-index-has-figure__link c-transit-fade u-tt-u">
                <a class="c-link-rect" href="/">
                  <div class="c-link-rect__label">Works<span class="c-icon-external"></span></div>
                </a>
              </div>
              <div class="p-index-has-figure__figure">
                <img src="~assets/img/pc/index/img_apparel.jpg" alt="">
              </div>
            </div>
          </div>
          <div class="p-index-section">
            <div class="p-index-section__in p-index-has-figure">
              <h2 class="p-index-has-figure__head u-tt-u">
                <div class="c-perspective u-tt-u">
                  <span class="c-noise-str c-noise-str--4 js-noise-str">R</span>
                  <span class="c-noise-str c-noise-str--1 js-noise-str">e</span>
                  <span class="c-noise-str c-noise-str--3 js-noise-str">s</span>
                  <span class="c-noise-str c-noise-str--3 js-noise-str">u</span>
                  <span class="c-noise-str c-noise-str--2 js-noise-str">m</span>
                  <span class="c-noise-str c-noise-str--4 js-noise-str">e</span>
                </div>
              </h2>
              <div class="p-index-has-figure__link c-transit-fade u-tt-u">Coming Soon...</div>
              <div class="p-index-has-figure__figure">
                <img src="~assets/img/pc/index/img_boost.jpg" alt="">
              </div>
            </div>
          </div>
          <div class="p-index-section">
            <div class="p-index-section__in p-index-has-figure">
              <h2 class="p-index-has-figure__head u-tt-u">
                <div class="c-perspective u-tt-u">
                  <span class="c-noise-str c-noise-str--4 js-noise-str">C</span>
                  <span class="c-noise-str c-noise-str--1 js-noise-str">o</span>
                  <span class="c-noise-str c-noise-str--3 js-noise-str">n</span>
                  <span class="c-noise-str c-noise-str--2 js-noise-str">t</span>
                  <span class="c-noise-str c-noise-str--3 js-noise-str">a</span>
                  <span class="c-noise-str c-noise-str--1 js-noise-str">c</span>
                  <span class="c-noise-str c-noise-str--4 js-noise-str">t</span>
                </div>
              </h2>
              <div class="p-index-has-figure__link c-transit-fade u-tt-u">Coming Soon...</div>
              <div class="p-index-has-figure__figure">
                <img src="~assets/img/pc/index/img_boost.jpg" alt="">
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- <div class="p-custom-cursor" id="vue-custom-cursor" :style="setStyles">
      <div class="p-custom-cursor__plus" :class="{ 'is-show' : state === 1 }"></div>
      <div class="p-custom-cursor__grab-h" :class="{ 'is-show' : state === 2 || state === 3 }">
        <div class="p-custom-cursor__arrow p-custom-cursor__arrow--l" :class="{'is-grabbing' : state === 3 }"><img src="~assets/img/pc/common/arrow.svg" alt=""></div>
        <div class="p-custom-cursor__arrow p-custom-cursor__arrow--r" :class="{'is-grabbing' : state === 3 }"><img src="~assets/img/pc/common/arrow.svg" alt=""></div>
      </div>
      <div class="p-custom-cursor__grab-v" :class="{ 'is-show' : state === 4 || state === 5 }">
        <div class="p-custom-cursor__arrow p-custom-cursor__arrow--t" :class="{'is-grabbing' : state === 5 }"><img src="~assets/img/pc/common/arrow.svg" alt=""></div>
        <div class="p-custom-cursor__arrow p-custom-cursor__arrow--b" :class="{'is-grabbing' : state === 5 }"><img src="~assets/img/pc/common/arrow.svg" alt=""></div>
      </div>
      <div class="p-custom-cursor__prev" :class="{ 'is-show' : state === 6 }">
        <div class="p-custom-cursor__arrow p-custom-cursor__arrow--l"><img src="~assets/img/pc/common/arrow.svg" alt=""></div>
      </div>
      <div class="p-custom-cursor__next" :class="{ 'is-show' : state === 7 }">
        <div class="p-custom-cursor__arrow p-custom-cursor__arrow--r"><img src="~assets/img/pc/common/arrow.svg" alt=""></div>
      </div>
      <div class="p-custom-cursor__bg" :class="{ 'is-spread' : state === 1 || state === 2 || state === 4 || state === 6 || state === 7, 'is-grabbing' : state === 3 || state === 5 }"></div>
    </div> -->
    <canvas class="p-canvas-webgl" id="canvas-webgl"></canvas>
  </div>
</template>

<script>

export default {
  data() {
    return {
      currentKey: "blank",
      isValid: !1,
      currentId: "",
      isCurrentId: -1,
      isOveredHamburger: 0,
      isOpenedNavi: 0,
      isExpand: !1,
      isLoading: !0
    }
  },
  computed: {
    setLabelStyle: function() {
      if (!1 !== this.isValid) return "width:" + this.items[this.currentKey].width + "px"
    }
  },
  methods: {
    setLabel: function(t) {
        this.currentKey = t
    },
    mouseoverHamburger: function() {
        this.isOveredHamburger = 1
    },
    mouseoutHamburger: function() {
        this.isOveredHamburger = 2
    },
    toggleNavi: function() {
        1 === this.isOpenedNavi ? this.closeNavi() : this.openNavi()
    },
    openNavi: function() {
      this.isOpenedNavi = 1, t.contents.classList.add("is-opened-gnav"), e.wrap.classList.add("is-opened-gnav"), e.label.classList.add("is-opened-gnav")
    },
    closeNavi: function() {
      var n = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
      this.isOpenedNavi = 2, !1 === n && (t.contents.classList.remove("is-opened-gnav"), e.wrap.classList.remove("is-opened-gnav"), e.label.classList.remove("is-opened-gnav"))
    }
  }
}
</script>

<style lang="sass" scoped>

</style>