<template>
  <section>
    <div class="headings">
      <h4>#AJUDA</h4>
      <h2>Ficou alguma dúvida?</h2>
      <p>Nullam ornare eu nisi fringilla consectetur. Suspendisse potenti.</p>
    </div>

    <div class="boxes">
      <div class="line"></div>
      <div class="box">
        <div class="icon">
          <img
            src="../assets/imgs/smartphone.svg"
            alt="" />
        </div>
        <div class="content">
          <h3>Lorem ipsum dolor sit amet</h3>
          <p>
            Vestibulum faucibus risus eu mi volutpat, vel tristique dui rutrum.
          </p>
        </div>
        <img src="../assets/imgs/chevron.svg" />
      </div>
      <div class="line"></div>
      <div class="box">
        <div class="icon">
          <img
            src="../assets/imgs/smartphone.svg"
            alt="" />
        </div>
        <div class="content">
          <h3>Lorem ipsum dolor sit amet</h3>
          <p>
            Vestibulum faucibus risus eu mi volutpat, vel tristique dui rutrum.
          </p>
        </div>
        <img src="../assets/imgs/chevron.svg" />
      </div>
      <div class="line"></div>
      <div class="box">
        <div class="icon">
          <img
            src="../assets/imgs/smartphone.svg"
            alt="" />
        </div>
        <div class="content">
          <h3>Lorem ipsum dolor sit amet</h3>
          <p>
            Vestibulum faucibus risus eu mi volutpat, vel tristique dui rutrum.
          </p>
        </div>
        <img src="../assets/imgs/chevron.svg" />
      </div>
      <div class="line"></div>
    </div>
  </section>
</template>

<style scoped lang="scss">
  @use '../assets/css/colors';

  section {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 72px;
    @apply py-20 lg:px-20 xl:px-40;

    .headings {
      display: flex;
      align-items: center;
      flex-direction: column;
      gap: 8px;

      h4 {
        font-size: 18px;
        font-weight: 500;
        color: colors.$red;
      }

      h2 {
        font-family: Sora, sans-serif;
        font-size: 32px;
        font-weight: 600;
      }

      p {
        margin-top: 20px;
        font-size: 18px;
        color: #5f5f5f;
      }
    }

    .boxes {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 32px;

      .line {
        opacity: 0.1;
        height: 0.5px;
        width: 100%;
        background: colors.$red;
      }

      .box {
        display: flex;
        align-items: center;
        justify-content: space-between;
        gap: 28px;

        .icon {
          display: flex;
          align-items: center;
          justify-content: center;
          flex-shrink: 0;
          padding: 12px;
          border: 1px transparent;
          border-radius: 12px;
          background-color: white;
          @apply shadow-md;
        }

        .content {
          display: flex;
          flex-direction: column;
          justify-content: space-between;

          h3 {
            font-size: 18px;
            font-weight: 500;
            color: colors.$gray;
          }
        }
      }
    }
  }
</style>
