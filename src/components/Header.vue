<script setup lang="ts">
const isUserLoggedIn = ref(false);
</script>

<template>
  <header>
    <nav
      class="navbar navbar-expand-lg navbar-dark fixed-top"
      style="background-color: #99cd00"
    >
      <div class="container-fluid nav-padding">
        <a class="navbar-brand" href="<?php echo home_url(); ?>">
          <img
            class="me-1"
            src="/icons/iputone_logo_white.svg"
            style="width: 26px"
          />
          IPUT ONE
        </a>
        <button
          class="navbar-toggler border-0"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#top-nav"
          aria-controls="top-nav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse justify-content-end" id="top-nav">
          <ul class="navbar-nav">
            <li class="nav-item ms-2 me-2">
              <a
                class="nav-link active"
                aria-current="page"
                href="<?php echo $page_url->activity; ?>"
                >活動</a
              >
            </li>
            <li class="nav-item ms-2 me-2">
              <a
                class="nav-link active"
                aria-current="page"
                href="<?php echo $page_url->news; ?>"
                >ニュース</a
              >
            </li>
            <li class="nav-item ms-2 me-2">
              <a
                class="nav-link active"
                aria-current="page"
                href="<?php echo home_url('#circle'); ?>"
                >サークル</a
              >
            </li>
            <li class="nav-item ms-2 me-2">
              <a
                class="nav-link active"
                aria-current="page"
                href="<?php echo $page_url->faq; ?>"
                >FAQ</a
              >
            </li>
            <li class="nav-item ms-2 me-2">
              <a
                class="nav-link active"
                aria-current="page"
                href="<?php echo $page_url->contact; ?>"
                >お問い合わせ</a
              >
            </li>
            <li>
              <hr class="border-top" />
            </li>
            <li class="nav-item ms-2 me-2 d-flex justify-content-end">
              <a
                v-if="isUserLoggedIn"
                class="my-1"
                href="<?php echo $page_url->signup; ?>"
              >
                <button type="button" class="btn btn-light rounded-pill">
                  新規登録
                </button>
              </a>
            </li>
            <li class="nav-item ms-2 me-2 d-flex justify-content-end">
              <a
                v-if="isUserLoggedIn"
                class="my-1"
                href="<?php echo $page_url->mypage; ?>"
              >
                <button type="button" class="btn btn-light rounded-pill">
                  マイページ
                </button>
              </a>

              <a
                v-if="!isUserLoggedIn"
                class="my-1"
                href="<?php echo $page_url->login; ?>"
              >
                <button type="button" class="btn btn-light rounded-pill">
                  ログイン
                </button>
              </a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
</template>
