---
layout: page
permalink: /misc/
title: Misc.
nav: true
nav_order: 6
---

- My name, as typically pronounced in English: <button type="button" class="name-audio-btn" onclick="const a = document.getElementById('name-audio'); a.currentTime = 0; a.play().catch(e => console.error('name audio:', e));" aria-label="Play the English pronunciation of Akiho" title="Play"><i class="fa-solid fa-volume-high"></i></button> (sounds like <span class="nowrap">ah-KEE-hoh</span>, <span class="ipa">/ɑˈkiːhoʊ/</span>)
- In Japanese, my name is written <span lang="ja" class="ja">顕帆</span>: <span lang="ja" class="ja">顕</span> means "to become clearly visible," and <span lang="ja" class="ja">帆</span> means "sail."
- I was born and raised in Kyoto, Japan's ancient capital.
- I love pink (as you may have guessed from this website).
- I love anything transparent, especially glassware. I enjoy collecting it and taking photos of it. (My friends have always called me a magpie.)
- I enjoy studying world history.
- Favorite foods: Korean-style cold noodles and xiaolongbao.
- Favorite shows and films: *Attack on Titan*, *House of the Dragon*, *Dune: Prophecy*, *Mayday / Air Crash Investigation*, and *How to Train Your Dragon*. (Clearly, I like dragons.)
- I occasionally write a blog in Japanese: [teanotes.hatenablog.com](https://teanotes.hatenablog.com/)

<audio id="name-audio" src="{{ '/assets/audio/akiho.m4a' | relative_url }}" preload="auto"></audio>

<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Noto+Serif:wght@300&text=%2F%C9%91%CB%88ki%CB%90ho%CA%8A&display=swap">

<style>
  .name-audio-btn {
    font: inherit;
    color: var(--global-theme-color);
    background: none;
    border: none;
    padding: 0 0.2em;
    cursor: pointer;
  }
  /* Crimson Pro's IPA coverage is partial (ɑ/ʊ missing, ˈ/ː oddly drawn), so set the whole
     transcription in a light Noto Serif, loaded only for these glyphs, to keep it uniform. */
  .ipa {
    font-family: "Noto Serif", serif;
    font-weight: 300;
    font-size: 0.9em;
    white-space: nowrap; /* browsers may break before ˈ, splitting the transcription */
  }
  .nowrap {
    white-space: nowrap;
  }
  /* Japanese glyphs are full-height and look oversized next to Crimson Pro's small x-height; scale them down. */
  .ja {
    font-family: "Hiragino Mincho ProN", "Yu Mincho", "Noto Serif JP", serif;
    font-size: 0.85em;
    white-space: nowrap; /* CJK can break between any two characters; keep 顕帆 together */
  }
  .post article ul > li + li {
    margin-top: 0.6em;
  }
  .name-audio-btn:hover {
    opacity: 0.7;
  }
</style>
