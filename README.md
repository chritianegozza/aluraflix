# aluraflix
criar uma pagina paralela ao netflix em javascript


https://codepen.io/chritianegozza/pen/xxgVaKb 



html
<html>

<head>
    <title>
        Imersão Dev - Aula 04
    </title>
</head>

<body>
    <div class="container">
        <h1 class="page-title">
            Aluraflix
        </h1>
        <header>
     <ui> <nav>
                    <a href="#">Inicio</a>
                    <a href="#">Séries</a>
                    <a href="#">Filmes</a>
                    <a href="#">Documentários</a>
                </nav></ui>
       </header>
      
        <img src="https://www.alura.com.br/assets/img/imersoes/dev-2021/logo-imersao-aluraflix.svg" class="page-logo"
            alt="">
    </div>
    <a href="https://alura.com.br/" target="_blank">
        <img src="https://www.alura.com.br/assets/img/home/alura-logo.svg" alt="" class="alura-logo">
    </a>
  
  <main>
            <div class="filme-principal">
              <img class="align-self-end mr-3"srs="https://s2.glbimg.com/2C0hMRuCY_7NfDPjby4_Bjmq8Nc=/e.glbimg.com/og/ed/f/original/2018/03/22/avengers-infinity-war-official-poster-2018-4o.jpg"  height:400px width=500px>
                <div class="central">
                    <h3 class="Titulo">Seja bem vindo ao AluraFlix</h3>
                 <div class="conversor">
                   </main>
            <button role="button" class="botao"> 
                <i class="fas fa-play"></i>
                Assistir Agora
            </button>
            <button role="button" class="botao">
                <i class="fas fa-info-circle"></i>
                Mais Informações
            </button>
        </div>
    ></script>     
  
    <h2></h2>

  <button>Proximo</button>
  <button>Anterior</button>                 
                   
</html>



css
body {
  font-family: 'Roboto Mono',monospace;
  text-align:center;
  background-image: url('https://s2.glbimg.com/2C0hMRuCY_7NfDPjby4_Bjmq8Nc=/e.glbimg.com/og/ed/f/original/2018/03/22/avengers-infinity-war-official-poster-2018-4o.jpg');
  background-color: #000000;
  background-size: cover;
  background-position: center top;
  background-repeat: no-repeat;
}

.container {
  text-align: center;
  padding: 20px;
}

.header{
  color: #ffffff;
  margin-right: 5px;
}
.page-title {
  color: #ffffff;
  margin: 0 0 5px;
}

.page-subtitle {
  color: #red;
  margin-top: 5px;
}

.page-logo {
  width: 200px;
}

.alura-logo {
  width: 40px;
  position: absolute;
  top: 10px;
  right:10px;
}
.filme-principal{
  color: #ffffff;
  margin: 0 0 5px;
  
}


body > img {
  margin: 0 10px;
  border-radius: 10px;
  cursor:pointer;
}

.listaFilmes {
  direction: left
  transition: transform 2s ease  
    
}
select  {
  border-radius: 5px;
  border: none;
  outline: 0;
  font-family: 'Poppins';
  font-size: 14px !important;
}

button{
 background-color: rgba(0,0,0,.50);        border:none;
 color: white;
  
}

.botao{
    background-color: rgba(0,0,0,.50);                                        
    border:none;
    color: white;

    padding:15px 30px;
    margin-right: 15px;
    font-size: 12px;

    cursor: pointer;
    transition: .3s ease all;
}

.botao:hover{
    background-color:white;
    color:black;
}

.botao i{
    margin-right: 8px;
}





js

var myArray = ['Mulher Maravilha', 'Liga da Justiça', 'Thor Ragnarok', 'Homem de Ferro 2', 'Dr° Estranho','Guardiã da galaxia', 'Homem Aranha: Longe do lar'];


var listaFilmes = ["https://m.media-amazon.com/images/M/MV5BMTYzODQzYjQtNTczNC00MzZhLTg1ZWYtZDUxYmQ3ZTY4NzA1XkEyXkFqcGdeQXVyODE5NzE3OTE@._V1_UX182_CR0,0,182,268_AL_.jpg", "https://m.media-amazon.com/images/M/MV5BYjI3NDg0ZTEtMDEwYS00YWMyLThjYjktMTNlM2NmYjc1OGRiXkEyXkFqcGdeQXVyMTEyMjM2NDc2._V1_UX182_CR0,0,182,268_AL_.jpg", "https://m.media-amazon.com/images/M/MV5BMjMyNDkzMzI1OF5BMl5BanBnXkFtZTgwODcxODg5MjI@._V1_UX182_CR0,0,182,268_AL_.jpg", "https://m.media-amazon.com/images/M/MV5BMTM0MDgwNjMyMl5BMl5BanBnXkFtZTcwNTg3NzAzMw@@._V1_UX182_CR0,0,182,268_AL_.jpg","https://m.media-amazon.com/images/M/MV5BNjgwNzAzNjk1Nl5BMl5BanBnXkFtZTgwMzQ2NjI1OTE@._V1_UX182_CR0,0,182,268_AL_.jpg","https://m.media-amazon.com/images/M/MV5BNjM0NTc0NzItM2FlYS00YzEwLWE0YmUtNTA2ZWIzODc2OTgxXkEyXkFqcGdeQXVyNTgwNzIyNzg@._V1_UX182_CR0,0,182,268_AL_.jpg", "https://m.media-amazon.com/images/M/MV5BNTk4ODQ1MzgzNl5BMl5BanBnXkFtZTgwMTMyMzM4MTI@._V1_UX182_CR0,0,182,268_AL_.jpg" ]

for (var i = 0; i < listaFilmes.length; i++){


  document.write("<img src=" +  listaFilmes[i] + ">")
  
} 

