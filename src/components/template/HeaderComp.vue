<template>
  <div class="primeiraParte">
    <div class="content">
      <div class="jpg">
        <img class="logosul" src="src/imagens/logoSulTurismo.png" />
      </div>
      <div class="infoHeader">
        <div>
          <span>Quem somos</span>
        </div>
        <div>
          <span>Nossos serviços</span>
        </div>
        <div>
          <span>Contato</span>
        </div>
      </div>
    </div>
    <div class="info1">
      <div class="textInfo1">Somos especialistas em transporte escolar</div>
      <div>
        <hr />
      </div>
    </div>
  </div>
  <div class="linear"></div>
  <div class="segundaParte">
    <div class="leftSegundaParte">
      <div class="tituloSegundaParte">FRETAMENTOS DE ÔNIBUS</div>
      <div class="textoSegundaParte">
        A
        <span style="font-size: 1.4rem"> Sul turismo</span> investe em
        tecnologia, adquirindo o que a de mais novo, seguro e sofisticado no
        ramo de transporte terrestre de passageiros proporcionando a você,
        familiares e amigos, uma viagem com o conforto e a segurança que merece.
      </div>
      <div class="segundotituloSegundaParte">MONTAMOS SUA VIAGEM</div>
      <div class="segundotextoSegundaParte">
        Você sabia que a style
        <span style="font-size: 1.4rem"> Sul turismo</span> monta viagens
        personalizadas para grupos? Quer fazer aquela viagem em grupo? Montar
        aquela viagem da empresa para curtir um dia especial? Levar a família
        para conhecer um lugar novo? A
        <span style="font-size: 1.4rem"> Sul turismo</span> , te ajuda a montar
        a sua viagem em grupo! Solicite um orçamento via
        <a
          href="https://api.whatsapp.com/send?phone=5547996767651&text=Oi%20"
          target="_blank"
        >
          WhatsApp.</a
        >
      </div>
    </div>
    <div class="rightSegundaParte">
      <div class="form1">
        <img class="onibusum" src="src/imagens/onibus1.png" alt="" />
        <div class="form3">
          <img class="onibustres" src="src/imagens/onibus2.png" alt="" />
        </div>
      </div>
      <div class="form2">
        <img class="onibusdois" src="src/imagens/microonibus.png" alt="" />
      </div>
    </div>
  </div>
  <div class="parceira">
    <div class="tituloParceira">
      Somos empresa parceira do <br />
      Instituto Federal Catarinense
    </div>
  </div>
  <div class="terceiraParte">
    <div class="cotacao">
      Solicite uma cotação on-line.
      <hr class="hrcotacao" />
    </div>
    <div class="v-line"></div>
    <div class="formulario">
      <div class="tituloFormulario">Pedir um orçamento</div>
      <br />
      <div class="group">
        <input required="" type="text" class="input" />
        <span class="highlight"></span>
        <span class="bar"></span>
        <label>NOME:</label> <br />
      </div>
      <div class="group">
        <input required="" type="text" class="input" />
        <span class="highlight"></span>
        <span class="bar"></span>
        <label>CEP DE DESTINO:</label><br />
      </div>
      <div class="group">
        <input required="" type="text" class="input" />
        <span class="highlight"></span>
        <span class="bar"></span>
        <label>CEP DE ORIGEM:</label><br />
      </div>
      <div class="group">
        <input required="" type="number" class="input" />
        <span class="highlight"></span>
        <span class="bar"></span>
        <label>QUANTIDADE DE PESSOAS:</label><br />
      </div>
      <div class="group">
        <input required="" type="" class="input" />
        <span class="highlight"></span>
        <span class="bar"></span>
        <label>TELEFONE CONTATO:</label>
      </div>
      <button>
        <span>Enviar</span>
      </button>
    </div>
  </div>
</template>
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Arimo:wght@600&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Bangers&family=Roboto+Mono:ital,wght@1,700&display=swap");
head {
  margin: 0px;
}

body {
  margin: 0px;
}

.primeiraParte {
  height: 1000px;
  width: 100%;
  background-image: url("src/imagens/imgPrincipal.png");
  background-repeat: no-repeat;
  background-size: cover;
  z-index: 5;
  background-color: linear-gradient(
    180deg,
    rgba(0, 0, 0, 0.63) 0%,
    rgba(0, 0, 0, 0) 100%
  );
  opacity: 95%;
  border-radius: 25px;
}
.content {
  display: flex;
  align-items: center;
  background-color: rgb(0, 0, 0);
  height: 130px;
  justify-content: space-between;
  padding: 0 10%;
}
.logosul {
  width: 130px;
}
.infoHeader {
  color: #ffff;
  justify-content: space-between;
  margin: 0 10% 0 0;
  text-transform: uppercase;
  display: flex;
  font-family: "Arimo";
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 25px;
  margin: 0% 0 0 0;
  padding: 0;
  text-align: center;
}
.infoHeader :hover {
  color: #fa943a;
}
.infoHeader span {
  padding: 15px;
}
.info1 {
  background: rgba(0, 0, 0, 0.72);
  border-radius: 30px;
  width: 713px;
  height: 308px;
  margin: 14% 0 0 30%;
}
.textInfo1 {
  font-family: "Arimo";
  font-style: normal;
  font-weight: 700;
  font-size: 45px;
  line-height: 57px;
  color: #ffffff;
  text-align: center;
  padding: 10% 0 0 0;
}
hr {
  border: 1px solid #f5a200;
  width: 373px;
  height: 0px;
  margin: 5% 0 0 25%;
}
.hrcotacao {
  border: 2px solid #f5a200;
  background-color: #f5a200;
  width: 500px;
  height: 0px;
  margin: 1% 0 0 10%;
}
.segundaParte {
  background-color: white;
  display: flex;
  height: 700px;
  margin: 0;
}
.leftSegundaParte {
  display: block;
  height: 450px;
  width: 600px;
  margin: 5% 20% 0 8%;
}
.rightSegundaParte {
  display: flex;
}
.tituloSegundaParte {
  font-family: "Arimo";
  font-style: italic;
  font-weight: 700;
  font-size: 30px;
  line-height: 37px;
  color: #db6900;
  white-space: nowrap;
  padding: 2%;
  margin: 0 0% 0 0%;
}
.segundotituloSegundaParte {
  font-family: "Arimo";
  font-style: italic;
  font-weight: 700;
  font-size: 30px;
  line-height: 37px;
  color: #db6900;
  white-space: nowrap;
  padding: 2%;
  margin: 10% 0 0 25%;
}
.textoSegundaParte {
  font-family: "Arimo";
  font-style: italic;
  font-weight: 700;
  font-size: 22px;
  line-height: 23px;
  color: #000000;
  margin: 0 0% 0 3%;
}
.segundotextoSegundaParte {
  font-family: "Arimo";
  font-style: italic;
  font-weight: 700;
  font-size: 22px;
  line-height: 22px;
  color: #000000;
  margin: 0% 0 0 25%;
  padding: 2%;
}
.primerosform {
  display: flex;
}
.form1 {
  background: #f98425f7;
  border-radius: 20px;
  width: 156px;
  height: 214px;
  margin: 20% 0 0 0;
}
.form2 {
  background: #f98425f7;
  border-radius: 20px;
  width: 208px;
  height: 192px;
  margin: 70% 0 0 55%;
}
.form3 {
  background: #f98425f7;
  border-radius: 20px;
  width: 156px;
  height: 287px;
  margin: 40% 0 0 0;
}
.onibusum {
  margin: 0 30% 0 0%;
}
.segundaParteImagens {
  display: flex;
}
.parceira {
  height: 300px;
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url("src/imagens/ifc.png");
  background-repeat: no-repeat;
  background-size: cover;
}
.tituloParceira {
  font-family: "Arimo";
  font-style: italic;
  font-weight: 700;
  font-size: 40px;
  line-height: 41px;
  color: white;
  text-align: center;
  padding: 7% 0 0 0;
}
.terceiraParte {
  height: 1000px;
  display: flex;
}
.cotacao {
  font-family: "Arimo";
  font-style: normal;
  font-weight: 700;
  font-size: 45px;
  line-height: 60px;
  text-align: right;
  color: #000000;
  margin: 23% 0 0 11%;
  white-space: nowrap;
}
.v-line {
  border-left: thick solid #000;
  height: 70%;
  position: absolute;
  margin: 10% 0 0 53%;
}
.formulario {
  margin: 1% 0 0 17%;
}
.tituloFormulario {
  font-family: "Bangers", cursive;
  font-weight: 500;
  font-size: 60px;
  line-height: 75px;
  padding: 25px 0 0 0;
  color: #db6900;
}
.group {
  position: relative;
}

.input {
  font-size: 20px;
  padding: 55px 10px 10px 10px;
  display: block;
  width: 430px;
  border: none;
  border-bottom: 1px solid #515151;
  background: transparent;
  margin: 5% 0 0 0;
}

.input:focus {
  outline: none;
}

label {
  font-family: "Arimo";
  color: black;
  font-size: 20px;
  font-weight: 700;
  position: absolute;
  pointer-events: none;
  left: 5px;
  top: 10px;
  transition: 0.2s ease all;
  -moz-transition: 0.2s ease all;
  -webkit-transition: 0.2s ease all;
}

.input:focus ~ label,
.input:valid ~ label {
  top: -18px;
  font-size: 17px;
  color: black;
}

.bar {
  position: relative;
  display: block;
  width: 200px;
}

.bar:before,
.bar:after {
  content: "";
  height: 2px;
  width: 0;
  bottom: 1px;
  position: absolute;
  background: #db6900;
  transition: 0.2s ease all;
  -moz-transition: 0.2s ease all;
  -webkit-transition: 0.2s ease all;
}

.input:focus ~ .bar:before,
.input:focus ~ .bar:after {
  width: 225%;
}

.highlight {
  position: absolute;
  height: 60%;
  width: 100px;
  top: 25%;
  left: 0;
  pointer-events: none;
  opacity: 0.5;
}

.input:focus ~ .highlight {
  animation: inputHighlighter 0.3s ease;
}

@keyframes inputHighlighter {
  from {
    background: #ffffff;
  }

  to {
    width: 0;
    background: transparent;
  }
}
button {
  background: black;
  border: none;
  padding: 10px 20px;
  display: inline-block;
  font-size: 18px;
  font-weight: bold;
  width: 160px;
  text-transform: uppercase;
  cursor: pointer;
  transform: skew(-21deg);
  color: #ffffff;
  margin: 10% 0 0 32%;
}

button::before {
  content: "";
  position: absolute;
  top: 0;
  bottom: 0;
  right: 100%;
  left: 0;
  background-color: #db6900;
  color: black;
  opacity: 0;
  z-index: -1;
  transition: all 0.5s;
}

button:hover {
  background-color: black;
  color: black;
}

button:hover::before {
  left: 0;
  right: 0;
  opacity: 1;
}
.onibusum {
  margin: 35% 0% 0 0;
}
.onibustres {
  margin: 50% 0% 0 0;
}
a {
  font-weight: bold;
  text-decoration: none;
  color: #f98425f7;
  font-size: 1.4rem;
}
a:hover {
  color: #af5811f7;
}
</style>
<script>
export default {
  data() {
    return {
      visible: true,
    };
  },
  methods: {
    scrollTop: function () {
      this.intervalId = setInterval(() => {
        if (window.pageYOffset === 0) {
          clearInterval(this.intervalId);
        }
        window.scroll(100, window.pageYOffset - 150);
      }, 20);
    },
    scrollListener: function (e) {
      this.visible = window.scrollY > -550;
    },
  },
  mounted: function () {
    window.addEventListener("scroll", this.scrollListener);
  },
  beforeDestroy: function () {
    window.removeEventListener("scroll", this.scrollListener);
  },
};
</script>
