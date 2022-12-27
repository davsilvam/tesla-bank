<script setup>
  import { CheckBadgeIcon, UserCircleIcon } from '@heroicons/vue/24/outline'
</script>

<template>
  <section>
    <div class="headings">
      <h4>#AJUDA</h4>
      <h2>Ficou alguma dúvida?</h2>
      <p>Abaixo estão alguns tópicos que podem ajudar você.</p>
    </div>

    <div class="boxes">
      <div class="line"></div>
      <div class="box">
        <div class="left">
          <div class="icon">
            <img src="../assets/imgs/teslabank_logo.svg" />
          </div>
          <div class="content">
            <h3>Conheça a TeslaBank</h3>
            <p>
              Tópico com informações sobre a TeslaBank, objetivo e funcionários.
            </p>
          </div>
        </div>
        <img src="../assets/imgs/chevron.svg" />
      </div>
      <div class="line"></div>
      <div class="box">
        <div class="left">
          <div class="icon">
            <CheckBadgeIcon class="w-8 text-[#E51D37]" />
          </div>
          <div class="content">
            <h3>Serviços</h3>
            <p>
              Este tópico possui a lista de serviços fornecidos pela TeslaBank.
            </p>
          </div>
        </div>
        <img src="../assets/imgs/chevron.svg" />
      </div>
      <div class="line"></div>
      <div class="box">
        <div class="left">
          <div class="icon">
            <UserCircleIcon class="w-8 text-[#E51D37]" />
          </div>
          <div class="content">
            <h3>Abrir uma conta</h3>
            <p>Dificuldades em abrir a conta? Cheque este tópico.</p>
          </div>
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
    min-height: 110vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 72px;
    @apply py-20 px-10 xl:px-40;

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
      align-items: stretch;
      gap: 32px;

      .line {
        opacity: 0.1;
        height: 0.5px;
        width: 100%;
        background: colors.$red;
      }

      .box {
        cursor: pointer;
        display: flex;
        align-items: center;
        justify-content: space-between;
        gap: 28px;

        .left {
          display: flex;
          gap: 24px;

          .icon {
            width: 60px;
            height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-shrink: 0;
            padding: 12px;
            border: 1px transparent;
            border-radius: 12px;
            background-color: white;
            @apply shadow-md;

            img {
              height: 35px;
            }
          }

          .content {
            display: flex;
            flex-direction: column;
            justify-content: center;
            gap: 4px;

            h3 {
              font-size: 18px;
              font-weight: 500;
              color: colors.$gray;
            }

            p {
              font-size: 14px;
              color: #5f5f5f;
            }
          }
        }
      }
    }
  }
</style>
