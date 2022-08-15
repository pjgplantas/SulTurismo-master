<template>
  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
  />
  <div class="footer">
    <div class="col-1">
      CENTRAL <br />
      <i class="fa fa-phone" style="font-size: 18px; color: white"></i>
      <span> |</span>
      Telefone: (47) 3434-3434 | (47) 3434-3434 <br /><br />
      SAC <br />
      <i class="fa fa-phone" style="font-size: 18px; color: white"></i>
      <span> |</span>
      Telefone: (47) 99999-9999 <br /><br />
      COLETAS <br />
      <i class="fa fa-phone" style="font-size: 18px; color: white"></i>
      <span> |</span>
      Telefone: (47) 99999-9999
    </div>
    <div class="col-2">
      INFORMAÇÕES: <br />
      Posição de entrega e outros assuntos: <br /><br />
      <i class="fa fa-envelope" style="font-size: 18px; color: white"></i>
      <span> |</span>
      E-mail: atendimento@sulturismo.com.br <br /><br />
      Política de Privacidade
      <i class="fa fa-check-circle" style="font-size: 18px; color: white"></i>
      <br />
      Siga nossas redes sociais: <br />
      <i class="fa fa-instagram" style="font-size: 18px; color: white"></i>
      <span> |</span> <span></span>
      <a href="https://www.instagram.com/sulturismotransporte/" target="_blank"
        >Instagram</a
      >
      <br />
      <i class="fa fa-facebook" style="font-size: 18px; color: white"></i>
      <span> |</span> <span></span>
      <a
        href="https://www.facebook.com/pages/Sul-Turismo-Transporte-Executivo/509345286485400 "
        target="_blank"
      >
        Facebook</a
      >
    </div>
    <div class="pneu">
      <img src="src/imagens/pneu.png" alt="" height="170px" width="120px" />
    </div>
    <div class="uiverse">
      <span class="tooltip">TOPO</span>
      <span @click="scrollTop" v-show="visible">
        <i class="fa fa-chevron-up" style="font-size: 40px; color: black"></i>
      </span>
    </div>
  </div>
</template>
<style>
.footer {
  background-color: black;
  height: 280px;
  color: white;
  display: flex;
}
.col-1 {
  font-family: "Arimo";
  font-style: normal;
  font-weight: 700;
  font-size: 16px;
  line-height: 27px;
  color: #ffffff;
  margin: 2% 0 0 20%;
}
.col-2 {
  font-family: "Arimo";
  font-style: normal;
  font-weight: 700;
  font-size: 16px;
  line-height: 29px;
  color: #ffffff;
  margin: 1% 0 0 10%;
}
.pneu {
  margin: 3% 0 0 17%;
}
a {
  text-decoration: none;
  color: white;
}
a:hover {
  color: #c95c00;
}
.uiverse {
  position: relative;
  background: #ffffff;
  color: #000;
  padding: 15px;
  margin: 10px;
  border-radius: 10px;
  width: 30px;
  height: 20px;
  font-size: 17px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  cursor: pointer;
  transition: all 0.2s cubic-bezier(0.68, -0.55, 0.265, 1.55);
  margin: 1% 0 0 3%;
}

.tooltip {
  position: absolute;
  top: 0;
  font-size: 14px;
  background: #ffffff;
  color: #ffffff;
  padding: 5px 8px;
  border-radius: 5px;
  box-shadow: 0 10px 10px rgba(0, 0, 0, 0.1);
  opacity: 0;
  pointer-events: none;
  transition: all 0.3s cubic-bezier(0.68, -0.55, 0.265, 1.55);
  font-weight: bold;
  font-family: Georgia, "Times New Roman", Times, serif;
}

.tooltip::before {
  position: absolute;
  content: "";
  height: 8px;
  width: 8px;
  background: #000000;
  bottom: -3px;
  left: 50%;
  transform: translate(-50%) rotate(45deg);
  transition: all 0.3s cubic-bezier(0.68, -0.55, 0.265, 1.55);
}

.uiverse:hover .tooltip {
  top: -45px;
  opacity: 1;
  visibility: visible;
  pointer-events: auto;
}

svg:hover span,
svg:hover .tooltip {
  text-shadow: 0px -1px 0px rgba(0, 0, 0, 0.1);
}

.uiverse:hover,
.uiverse:hover .tooltip,
.uiverse:hover .tooltip::before {
  background: lightgray;
  color: black;
  box-shadow: 0 5px 5px lightgrey;
}
@media (max-width: 844px) {
  .footer {
    width: 100vh;
    height: 95vh;
    margin: 0;
    display: block;
    padding: 10px 0 0 0;
  }
  .col-1 {
    margin: 3% 0 0 10%;
    font-size: 13px;
    line-height: 20px;
  }
  .col-2 {
    margin: 5% 0 0 10%;
    font-size: 13px;
  }
  img {
    width: 100px;
    height: 150px;
    margin: 4% 0 0 0;
  }
  .uiverse {
    display: none;
  }
}
</style>

<script>
export default {
  data() {
    return {
      visible: false,
    };
  },
  methods: {
    scrollTop: function () {
      this.intervalId = setInterval(() => {
        if (window.pageYOffset === 0) {
          clearInterval(this.intervalId);
        }
        window.scroll(0, window.pageYOffset - 50);
      }, 20);
    },
    scrollListener: function (e) {
      this.visible = window.scrollY > 150;
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
