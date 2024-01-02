<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quer Casar comigo Julia?</title>
    <style>
        body {
            background-color: red;
            overflow: hidden;
        }
        h1{
            text-align: center;
            text-transform: uppercase;
            color: #fff;
        }
        .center{
            display: flex;
            margin: 0;
            justify-content: center;
            align-items: center;
            height: 30vh;
        }
        a{
            text-decoration: none;
            color: inherit;
        }
        .btn{
            display: flex;
            justify-content: center;
            align-items: center;
        }
        button{
            margin: 0 20px;
            color: #000;
            background-color: #fff;
            border: none;
            border-radius: 5px;
            font-size: 2rem;
            cursor: pointer;
        }
        .img{
            display: block;
            background-image: url('https://uniquebox.vteximg.com.br/arquivos/ids/158482/pedido-de-namoro_front.png?v=636936274247270000');
            background-size: cover;
            background-color: #fff;
            background-repeat: no-repeat;
            background-position: center;
            height: 300px;
            width: 300px;
            margin: 0 auto;
            margin-bottom: 50px;
            border-radius: 50%;
        }
        
    </style>
</head>
<body>
    <div class="center">
        <h1>Quer Casar comigo Júlia?</h1>
    </div>
    <div class="img"></div>
    <div class="btn">
        <button id="sim"><a href="https://m.youtube.com/watch?v=dp4cLPTcVU4&pp=ygUlbXVzaWNhIGRlIGNhc2FtZW50byBlbnRyYWRhIGRhIG5vaXZhIA%3D%3D">Sim</a></button>
        <button id="nao">Não</button>
    </div>
</body>
<script>
    const naoBtn = document.querySelector('#nao');
    const simBtn = document.querySelector('#sim');
    const img = document.querySelector('.img');

    simBtn.addEventListener('mouseover', ()=>{
        img.style.backgroundImage = "url('https://uniquebox.vteximg.com.br/arquivos/ids/158485/pedido-de-namoro_right.png?v=636936274608270000')"
    });
    simBtn.addEventListener('mouseout', ()=>{
        img.style.backgroundImage = "url('https://uniquebox.vteximg.com.br/arquivos/ids/158482/pedido-de-namoro_front.png?v=636936274247270000')"
    });
    naoBtn.addEventListener('mouseover', ()=>{
       naoBtn.style.position = 'absolute';
        naoBtn.style.left = Math.floor(Math.random() * window.innerWidth) + "px";
        naoBtn.style.top = Math.floor(Math.random() * window.innerHeight) + "px"; 
    });
</script>
</html>
