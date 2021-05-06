<template>
  <div :class="$style.container">
    <div>
      <main class="my-5">
        <h1 :class="$style.title">Liel.la!</h1>
        <hr />
        <h2 :class="$style.subtitle">
          私を<span :class="$style.subtitlePoint">叶</span>える物語
        </h2>
      </main>
      <aside class="my-3">
        <b-button
          variant="primary"
          size="sm"
          :class="$style.btnTwitter"
          href="https://twitter.com/hashtag/%E5%A7%8B%E3%81%BE%E3%82%8A%E3%81%AF%E3%81%BF%E3%82%93%E3%81%AA%E3%81%AE%E7%A9%BA"
        >
          <img src="~/assets/images/twitter.svg" :class="$style.twitterIcon" />
          #始まりはみんなの空
        </b-button>
      </aside>
      <aside class="my-3" :class="$style.links">
        <b-button
          variant="primary"
          :class="$style.btnTwitter"
          href="https://twitter.com/intent/tweet?url=https://liel.la/&text=%E7%A7%81%E3%82%92%E5%8F%B6%E3%81%88%E3%82%8B%E7%89%A9%E8%AA%9E&hashtag=始まりはみんなの空"
        >
          <img src="~/assets/images/twitter.svg" :class="$style.twitterIcon" />
          ツイート
        </b-button>
        <b-button
          variant="outline-success"
          href="https://lovelive-anime.jp/yuigaoka/"
        >
          公式ウェブサイトへ
        </b-button>
      </aside>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style module>
.container {
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 600;
  font-size: 100px;
  color: #a5469b;
  letter-spacing: 0.1rem;
}

.subtitle {
  font-family: serif;
  margin-right: -1rem;
  letter-spacing: 1rem;
}

.subtitlePoint {
  color: #e4007f;
}

.links {
  display: inline-flex;
  gap: 0 1rem;
}

.btnTwitter {
  border-color: #1da1f2;
  background-color: #1da1f2;
  display: inline-flex;
}

.twitterIcon {
  width: 1.5em;
  height: 1.5em;
  margin-right: 0.2rem;
}
</style>
