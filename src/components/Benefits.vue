<template>
  <section>
    <img
      class="wave"
      src="../assets/imgs/benefits_wave.svg" />
    <div class="headings">
      <h4>#INOVAÇÃO</h4>
      <h2>
        Quais as vantagens <br />
        de usar <span>TeslaBank</span>?
      </h2>
    </div>
    <div class="cards">
      <div class="card">
        <div>
          <img src="../assets/imgs/credit-card.svg" />
          <h3>Cartão TeslaBank</h3>
          <p>
            O Cartão TeslaBank conta com anuidade zero, além de cashback sobre
            suas compras e disponibilidade para pagamentos internacionais!
          </p>
        </div>
        <a>ADQUIRA O SEU</a>
      </div>
      <div class="card">
        <div>
          <img src="../assets/imgs/shopping-cart.svg" />
          <h3>Investimentos</h3>
          <p>
            A TeslaBank trabalha com as melhores taxas do mercado, para que você
            possa criar um portfólio para o seu perfil de investidor sem medo.
          </p>
        </div>
        <a>VEJA OS INVESTIMENTOS</a>
      </div>
      <div class="card">
        <div>
          <img src="../assets/imgs/clock.svg" />
          <h3>Atendimento 24h</h3>
          <p>
            Nós temos antedimento exclusivo 24h. Comunique-se por chat ou
            ligação e estaremos prontos para te atender da melhor forma.
          </p>
        </div>
        <a>FALE COM A CENTRAL</a>
      </div>

      <div class="lg:row-start-2 lg:col-start-2 card">
        <div>
          <img src="../assets/imgs/shield.svg" />
          <h3>Segurança</h3>
          <p>
            A TeslaBank preza pela sua segurança e a do seu dinheiro. Conte com
            autenticação de dois fatores, login com biometria e muito mais.
          </p>
        </div>
        <a>PROTEJA SUA CONTA</a>
      </div>
      <div class="lg:row-start-2 lg:col-start-3 card">
        <div>
          <img src="../assets/imgs/percent.svg" />
          <h3>Sem taxas</h3>
          <p>
            O banco que corta todas as taxas pelo bem-estar do cliente? Só na
            TeslaBank. Não há taxa alguma de saque, anuidade, nem segunda via.
          </p>
        </div>
        <a>CONFIRA OS DADOS</a>
      </div>
      <div class="lg:row-start-2 lg:col-start-4 card">
        <div>
          <img src="../assets/imgs/gift.svg" />
          <h3>Receba prêmios</h3>
          <p>
            Nossa equipe adora presentear seus clientes nos melhores momentos.
            Receba prêmios e brindes, seja feliz e venha para a TeslaBank.
          </p>
        </div>
        <a>TORNE-SE CLIENTE</a>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
  @use '../assets/css/colors';

  section {
    position: relative;
    min-height: 110vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 52px;
    background-color: #f2f4fd;
    @apply py-32 px-10 xl:px-40;

    .wave {
      position: absolute;
      top: 30%;
      left: 0;
    }

    .headings {
      z-index: 10;
      display: flex;
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
        line-height: 45px;

        span {
          color: colors.$red;
        }
      }
    }

    .cards {
      z-index: 10;
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      grid-template-rows: repeat(2, 1fr);
      @apply max-sm:grid-cols-1 max-lg:grid-cols-2 max-lg:grid-rows-3;
      gap: 32px;

      .card {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        padding: 16px;
        background-color: white;
        @apply shadow-md;

        div {
          color: colors.$gray;
          padding-bottom: 16px;

          img {
            width: 35px;
            padding-bottom: 12px;
          }

          h3 {
            font-family: Sora, sans-serif;
            font-size: 18px;
            font-weight: 500;
          }

          p {
            opacity: 0.75;
            text-align: justify;
            font-size: 14px;
          }
        }

        a {
          cursor: pointer;
          justify-self: flex-end;
          text-decoration: underline;
          font-size: 14px;
          font-weight: 600;
          color: colors.$red;
        }
      }
    }
  }
</style>
