# Projeto-Site-de-vendas
esse site é composto somente por HTML e CSS, é um projeto que fiz para por em prática oque eu aprendi, site de vendas do filme do homem aranha

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Homem Aranha</title>
    <link rel="shortcut icon" href="./spider-removebg-preview.png">
</head>
<body>
    <link rel="stylesheet" href="./style.css">


    <header>
        <a class="imagem" href="./index.html">
            <img id="logo" src="./logo_homem_aranha_de_volta_ao_lar__ingles__by_samukabrenner16_dfkodyo-fullview-removebg-preview.png">
        </a>
        
        <nav>
                <ul>
                   <a href="./index.html">
                    <li>Home</li>
                    </a>
                    <a href="./contato.html">
                        <li>Contacts</li>
                    </a>
                    <a href="./fotos.html">
                        <li>Photos</li>
                    </a>
                   <a href="./comentarios.html">
                       <li>Comments</li>
                   </a>
            </ul>
        </nav>
    </header>
    <div id="banner"></div>

    <div id="trailer-container">
      <div id="content">
        <video controls class="trailer">
        <source src="Homem-Aranha - Sem Volta Para Casa _ Trailer Teaser Oficial Dublado.mp4" type="video/mp4">
        </video>
        
        <div class="sipnose">
            <p class="descricao">
                In Spider-Man: No Way Home, Peter Parker (Tom Holland) will need to deal with the consequences
                 of his identity as the world's most beloved hero after it was revealed by the Daily Bugle report.
                
                
            </p>
            <button class="botao">Buy ticket</button>
        </div>
    </div>
    </div> 

    <div class="actor-cards">
      <div class="card-content">
         <div class="card baner-1">Tom Holland-Spider man</div>
         <div  class="card baner-2">Andrew Garfield-Spider man</div>
         <div  class="card baner-3">Tobey Maguire-Spider man</div>
      </div>
    </div>

    <footer> 
       
        
        <nav class="footer-navegation">
            <ul class="footer-list">
                <a href="./index.html">
                    <li>Home</li>
                </a>
                <a href="./contato.html">
                    <li>Contacts</li>
                </a>
                <a href="./fotos.html">
                    <li>Photos</li>
                </a>
                <a href="./comentarios.html">
                    <li>Comments</li>
                </a>
            </ul>
        </nav>
        <img id="logo" src="./logo_homem_aranha_de_volta_ao_lar__ingles__by_samukabrenner16_dfkodyo-fullview-removebg-preview.png">
        <span>
            All rights reserved ©
        </span>
        <span>
            developed by: Caio Cabral P.
        </span>
    </footer>
</body>
</html>



CSS


@import url('https://fonts.googleapis.com/css2?family=Kdam+Thmor+Pro&display=swap');



*{margin:0px;
padding:0px;
background-color: black;
list-style: none;
text-decoration: none;}


header{height:90px;
display: flex;
justify-content: space-around;
align-items: center;}

nav{width:60%;}

ul{display: flex;
width:100%;
justify-content: space-between;}

li{list-style: none; color: red;
cursor:pointer;
font-size: 19px;
transition: 0.5s;font-family:"Kdam Thmor Pro",sans-serif;}

li:hover{color: white;}


#logo{width:150px;
      height:auto;}

#banner{
    background-image: url("https://images8.alphacoders.com/131/1317672.jpg");
    background-position: 50% 50%;
    background-size:cover;
    width:100%;
    height:700px;
}


#trailer-container{
    width:100%;
    height:400px;
    display: flex;
justify-content:center;
}

#content{
    width:60%;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.trailer{width:50%; margin-right: 20px; margin-bottom: 68px;
}

#sinopse{width:50%;
    display: flex;
    flex-direction: column;
    justify-content:
    space-between;
    margin-left: 30px;}

.descricao{color: white;
    font-size: 19px;
    font-family:"Kdam Thmor Pro",sans-serif;
    width:70%;}

.botao{
    width:200px;
       height:60px;
background-color:red;
color: white;
padding: 8px 10px;
border-radius: 5px;
cursor:pointer;
transition: 0.5s;
font-size: 18px;
display: flex;
justify-content: center;
align-items: center;
font-weight: bold;
border: none;
outline:none;
margin-top: 25px;}


.botao:hover{
    background-color:white;
    color:black; transition: .6s; width: 230px;
}

.actor-cards{
    width:100%;
    display: flex;
    justify-content: center;
    margin-top: 50px;
    
    
}

.card-content{
    width:90%;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
}

.card{
    width:92%;
       height:600px;
background-size:cover;
background-position:50% 50%;
border-radius: 5px;
cursor:pointer;
transition: 1s;
display: flex;flex-direction: column;
justify-content: flex-end;
padding: 20px 10px;
color:white;
font-size: 18px;
font-family:"Kdam Thmor Pro",sans-serif;
}

.card:hover{
    transform: scale(1.02);
}

.baner-1{background-image: url("https://rukminim2.flixcart.com/image/850/1000/l1whaq80/poster/b/a/v/medium-tom-holland-spider-man-no-way-home-matte-finish-poster-original-imagdcwxv2demwvw.jpeg?q=90");}


.baner-2{background-image:url("https://i.pinimg.com/originals/70/c9/7e/70c97e0507144b27a3eac157584f5cb9.png");}

.baner-3{background-image:url("https://i.redd.it/j89b97ujcyz71.jpg");}


footer{
    height:300px;
    margin-top: 50px;
    display: flex;
    flex-direction: column;
align-items: center;
justify-content: space-around;}


span{
    color: white;
font-family: "Kdam Thmor Pro",sans-serif; margin-bottom: 20px; padding: 20px;}

.footer-navegation{
    display: none;
}

.footer-list{display: flex;flex-direction: column; align-items: center;}


.img{width:150px; position: relative; margin-top: 10px;}



@media(max-width: 768px){
    .footer-navegation{display: block;}
    nav{display: none;} 

    #banner{background-position: 80%;}

    #trailer-container{
    width:100%;
    height:400px;
    display: flex;
    flex-direction: column;
    }

    #content{
        width:95%;
        display: flex;
        flex-direction: column;
    }
    .trailer{
        width:100%;
        
    }
    .sipnose{
        width:100%;
        display: flex;
        flex-direction: column;
        display: flex;
        justify-content: space-between;
    }
    .descricao{width:100%;}

    .botao{width: 100%;
    margin-top: 30px;}

    .card-content{grid-template-columns: 1fr;
    margin-top: 150px;}
}
