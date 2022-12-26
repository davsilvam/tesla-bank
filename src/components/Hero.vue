<template>
  <section>
    <img
      class="line_1"
      src="../assets/imgs/line.svg" />
    <img
      class="line_2"
      src="../assets/imgs/line-two.svg" />
    <div class="left_side">
      <h1>
        TeslaBank <br />
        Banco 100% digital
      </h1>
      <h2>Abrir uma conta digital nunca foi tão simples!</h2>
      <div>
        <button class="open_button">
          Abrir uma conta
          <img src="../assets/imgs/arrow-right.svg" />
        </button>
        <div>
          <button>
            <img src="../assets/imgs/apple-store.svg" />
          </button>
          <button>
            <img src="../assets/imgs/play-store.svg" />
          </button>
        </div>
      </div>
    </div>
    <div class="right_side">
      <img src="../assets/imgs/cards.svg" />
    </div>
  </section>
</template>

<style scoped lang="scss">
  @use '../assets/css/colors';

  section {
    position: relative;
    width: 100%;
    display: flex;

    .line_1,
    .line_2 {
      position: absolute;
      @apply max-lg:hidden;
    }

    .line_1 {
      top: 15%;
    }

    .line_2 {
      right: 0;
      bottom: 5%;
    }

    .left_side,
    .right_side {
      width: 50%;
      min-height: 110vh;
      display: flex;
      justify-content: center;
    }

    .left_side {
      flex-direction: column;
      background-color: #f2f4fd;
      @apply max-lg:w-full px-10 xl:px-40;

      h1 {
        font-family: Sora, sans-serif;
        z-index: 10;
        padding-bottom: 24px;
        font-size: 48px;
        font-weight: 700;
        color: colors.$red;
      }

      h2 {
        opacity: 0.75;
        padding-bottom: 80px;
        font-size: 18px;
        font-weight: 500;
        color: colors.$gray;
      }

      div {
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        gap: 32px;

        .open_button {
          display: flex;
          align-items: center;
          gap: 12px;
          padding: 16px 32px;
          font-size: 18px;
          font-weight: 600;
          color: white;
          background-image: colors.$gradient;
        }

        .open_button + button {
          margin-left: 8px;
        }
      }
    }

    .right_side {
      align-items: center;
      background-image: colors.$gradient;
      @apply max-lg:hidden;

      img {
        z-index: 10;
        width: 75%;
      }
    }
  }
</style>
