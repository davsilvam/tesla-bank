<template>
  <section>
    <div class="left_side">
      <img src="../assets/imgs/cell.svg" />
    </div>
    <div class="right_side">
      <div>
        <h2>Abra sua conta <span>gratuita</span>!</h2>
        <p>
          Envie e receba dinheiro de forma mais prática e rápida. Faça Pix, TEDs
          e transferências com agendamento para todos os bancos sem pagar nada.
        </p>
      </div>
      <div class="topics">
        <div class="topic">
          <div class="icon">
            <img
              src="../assets/imgs/dollar-sign.svg"
              alt="" />
          </div>
          <div class="content">
            <h3>Seu dinheiro rendendo mais</h3>
            <p>Rendem mais que a poupança e você resgata quando quiser.</p>
          </div>
        </div>
        <div class="topic">
          <div class="icon">
            <img
              src="../assets/imgs/smartphone.svg"
              alt="" />
          </div>
          <div class="content">
            <h3>Conta digital 100% grátis</h3>
            <p>
              Transferências, boletos de depósito e outros serviços gratuitos.
            </p>
          </div>
        </div>
        <div class="topic">
          <div class="icon">
            <img
              src="../assets/imgs/smile.svg"
              alt="" />
          </div>
          <div class="content">
            <h3>Cartão sem anuidade</h3>
            <p>
              Conta digital com cartão de crédito sem anuidade e sem
              complicação.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
  @use '../assets/css/colors';

  section {
    width: 100%;
    min-height: 110vh;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 160px;
    @apply max-lg:flex-col max-lg:gap-20 md:px-40 px-10 xl:px-40 py-20;

    .left_side {
      width: 50%;
      @apply max-lg:w-full;
      display: flex;
      align-items: center;
      justify-content: center;

      img {
        width: 320px;
        @apply max-lg:w-[240px];
      }
    }

    .right_side {
      width: 50%;
      @apply max-lg:w-full max-lg:items-center;
      display: flex;
      flex-direction: column;
      gap: 56px;

      & > div {
        display: flex;
        flex-direction: column;
        gap: 16px;

        h2 {
          font-family: Sora, sans-serif;
          font-size: 32px;
          font-weight: 600;
          color: colors.$gray;

          span {
            color: colors.$red;
          }
        }

        p {
          opacity: 0.75;
          font-size: 18px;
          color: colors.$gray;
        }
      }

      .topics {
        display: flex;
        flex-direction: column;
        gap: 32px;

        .topic {
          display: flex;
          align-items: center;
          gap: 20px;

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
            gap: 4px;

            h3 {
              font-size: 18px;
              font-weight: 600;
            }

            p {
              opacity: 0.75;
              font-size: 14px;
            }
          }
        }
      }
    }
  }
</style>
