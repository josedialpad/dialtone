---
title: Background colors
desc: Utilities for setting background colors.
---

<aside class="d-notice d-notice--warning d-mt24 d-wmx100p" role="status" aria-hidden="false">
  <div class="d-notice__icon">
    <dt-icon name="alert-triangle"></dt-icon>
  </div>
  <div class="d-notice__content d-stack4">
    <p class="d-notice__message">
      Before using background color utilities, first consider <router-link to="/design/colors/#surface">semantic surface colors</router-link>.
    </p>
  </div>
</aside>

## Usage

Use `d-bgc-{color}` to set an element's background color.

<code-well-header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-purple-100 d-bgo50 d-w100p d-hmn102" custom>
  <div class="d-fs-200 d-p16 d-bar4 d-bgc-purple-300">The quick brown fox jumps over the lazy dog.</div>
</code-well-header>

```html
<div class="d-bgc-purple-300">...</div>
```

## Changing opacity

Use `d-bgo{stop}` to change an element's background color opacity. You can also change the background color opacity on `:hover`, `:focus`, `:focus-visible`, or in dark mode by using the respective `h:d-bgo{stop}`, `f:d-bgo{stop}`, `fv:d-bgo{stop}`, or `d:d-bgo{stop}` prefixes.

<code-well-header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-green-100 d-bgo50 d-w100p d-hmn102 d-stack8" custom>
  <div class="d-fl-center d-p16 d-bgc-green-200 d-bar4 d-fs-300 d-fw-bold">100%</div>
  <div class="d-fl-center d-p16 d-bgc-green-200 d-bgo99 d-bar4 d-fs-300 d-fw-bold">99%</div>
  <div class="d-fl-center d-p16 d-bgc-green-200 d-bgo95 d-bar4 d-fs-300 d-fw-bold">95%</div>
  <div class="d-fl-center d-p16 d-bgc-green-200 d-bgo90 d-bar4 d-fs-300 d-fw-bold">90%</div>
  <div class="d-fl-center d-p16 d-bgc-green-200 d-bgo75 d-bar4 d-fs-300 d-fw-bold">75%</div>
  <div class="d-fl-center d-p16 d-bgc-green-200 d-bgo50 d-bar4 d-fs-300 d-fw-bold">50%</div>
  <div class="d-fl-center d-p16 d-bgc-green-200 d-bgo25 d-bar4 d-fs-300 d-fw-bold">25%</div>
  <div class="d-fl-center d-p16 d-bgc-green-200 d-bgo10 d-bar4 d-fs-300 d-fw-bold">10%</div>
  <div class="d-fl-center d-p16 d-bgc-green-200 d-bgo0 d-bar4 d-fs-300 d-fw-bold">0%</div>
</code-well-header>

```html
<p class="d-bgc-green-200">...</p>
<p class="d-bgc-green-200 d-bgo99">...</p>
<p class="d-bgc-green-200 d-bgo95">...</p>
<p class="d-bgc-green-200 d-bgo90">...</p>
<p class="d-bgc-green-200 d-bgo75">...</p>
<p class="d-bgc-green-200 d-bgo50">...</p>
<p class="d-bgc-green-200 d-bgo25">...</p>
<p class="d-bgc-green-200 d-bgo10">...</p>
<p class="d-bgc-green-200 d-bgo0">...</p>
```

## Hover

Use `h:d-bgc-{color}` to change an element's `:hover` state background color.

<code-well-header class="d-fl-center d-p24 d-bgc-green-100 d-bgo50 d-w100p d-hmn102" custom>
  <button type="button" class="d-p16 d-bar4 d-fs-200 d-bgc-green-100 h:d-bgc-green-200 d-ba d-bc-transparent">Hover over me</button>
</code-well-header>

```html
<button class="d-bgc-green-100 h:d-bgc-green-200">...</button>
```

## Focus

Use `f:d-bgc-{color}` to change an element's `:focus` and `:focus-within` state background color.

<code-well-header class="d-fl-center d-p24 d-bgc-black-200 d-w100p d-hmn102" custom>
  <button class="d-p16 d-bar4 d-fs-200 d-fc-black-800 d-bgc-transparent f:d-fc-red-200 f:d-bgc-red-200 f:d-bgo25 d-ba d-bc-transparent">Click on me</button>
</code-well-header>

```html
<button class="d-bgc-transparent f:d-fc-red-200 f:d-bgc-red-200 f:d-bgo25">...</button>
```

## Focus visible

Use `fv:d-bgc-{color}` to change an element's `:focus-visible` state background color [only when focused by keyboard].

<code-well-header class="d-fl-center d-p24 d-bgc-black-200 d-w100p d-hmn102" custom>
  <button class="d-p16 d-bar4 d-fs-200 d-fc-black-800 d-bgc-transparent fv:d-fc-red-200 fv:d-bgc-red-200 fv:d-bgo25 d-ba d-bc-transparent">Focus on me</button>
</code-well-header>

```html
<button class="d-bgc-transparent fv:d-fc-red-200 fv:d-bgc-red-200 fv:d-bgo25">...</button>
```

<script setup>
  import colors from '@data/colors.json';
</script>

## Classes

<div class="d-h464 d-of-y-scroll d-bb d-bc-black-200">
  <utility-class-table>
    <template #content>
      <tbody>
          <tr>
              <th scope="row" class="d-ff-mono d-fc-purple-400 d-fw-normal d-fs-100">.d-bgc-transparent</th>
              <td>
                  <div class="d-d-flex d-jc-space-between d-ai-center">
                      <div class="d-fl-grow1 d-ff-mono d-fs-100">
                          background-color: transparent !important;
                      </div>
                      <div class="d-fl-shrink0 d-m4 d-ml16 d-h32 d-w32 d-bar4 d-bgc-transparent d-ba d-bc-black-100"></div>
                  </div>
              </td>
          </tr>
          <tr>
              <th scope="row" class="d-ff-mono d-fc-purple-400 d-fw-normal d-fs-100">.d-bgc-unset</th>
              <td>
                  <div class="d-d-flex d-jc-space-between d-ai-center">
                      <div class="d-fl-grow1 d-ff-mono d-fs-100">
                          background-color: unset !important;
                      </div>
                      <div class="d-fl-shrink0 d-m4 d-ml16 d-h32 d-w32 d-bar4 d-bgc-unset d-ba d-bc-black-100"></div>
                  </div>
              </td>
          </tr>
          <tr>
              <th scope="row" class="d-ff-mono d-fc-purple-400 d-fw-normal d-fs-100">.d-bgc-white</th>
              <td>
                  <div class="d-d-flex d-jc-space-between d-ai-center">
                      <div class="d-fl-grow1 d-ff-mono d-fs-100">
                          --bgo: 100%;<br/>
                          background-color: hsla(var(--white-h) var(--white-s) var(--white-l) / var(--bgo)) !important;
                      </div>
                      <div class="d-fl-shrink0 d-m4 d-ml16 d-h32 d-w32 d-bar4 d-bgc-white d-ba d-bc-black-100"></div>
                  </div>
              </td>
          </tr>
      </tbody>
      <tbody v-for="{ color, stops } in colors">
        <tr v-for="{ stop } in stops">
            <th scope="row" class="d-ff-mono d-fc-purple-400 d-fw-normal d-fs-100">.d-bgc-{{ color }}-{{ stop }}</th>
            <td>
                <div class="d-d-flex d-jc-space-between d-ai-center">
                    <div class="d-fl-grow1 d-ff-mono d-fs-100">
                        --bgo: 100%;<br/>
                        background-color: hsla(var(--{{ color }}-{{ stop }}-h) var(--{{ color }}-{{ stop }}-s) var(--{{ color }}-{{ stop }}-l) / var(--bgo)) !important;
                    </div>
                    <div
                      class="d-fl-shrink0 d-m4 d-ml16 d-h32 d-w32 d-bar4 d-ba d-bc-black-100"
                      :class="`d-bgc-${color}-${stop}`"
                    />
                </div>
            </td>
        </tr>
      </tbody>
    </template>
  </utility-class-table>
</div>
