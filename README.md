# Desafio-2---correção

Index.html

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projeto Blog</title>
    <link rel="stylesheet" href="./styles.css">
    <script src="https://kit.fontawesome.com/6fccb2eb21.js" crossorigin="anonymous"></script>
</head>
<body>
    <header id="cabecalho">
        <nav class="wrapper flex">
            <h3>Logo Blog</h3>
            <div class="links_menu">
                <a href="#" class="link_ativo">blog</a>
                <a href="#">contato</a>
            </div>
        </nav>
    </header>
    <main>
        <div class="wrapper" id="postagens">
            <article class="post">
                <header class="cabecalho_post flex">
                    <p>14 de fev, 2022</p>
                    <i class="far fa-heart"></i>
                </header>
                <div class="conteudo_post">
                    <h2>Titulo post 1</h2>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Doloribus, architecto dolorum. Minima sunt eveniet consectetur iusto adipisci mollitia placeat. Ea qui iste possimus at consequatur, sapiente voluptatibus quia voluptatem sunt.</p>
                </div>
            </article>
        </div>
    </main>
    <footer>
        <p>&copy; Todos os direitos reservados.</p>
    </footer>
</body>
</html>

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

style.css

@import url('https://fonts.googleapis.com/css2?family=Lexend+Deca:wght@100;200;300;400;500;600;700;800;900&display=swap');

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
h2, p, a{
    font-family: 'Lexend Deca', sans-serif;
}

a{
    text-decoration: none;
    color: inherit
}

.wrapper{
    width: 60%;
    max-width: 900px;
    margin: 0 auto;
}
.flex{
    display: flex;
    justify-content: space-between;
    align-items: center;
}
#cabecalho{
    background: linear-gradient(90deg, #DB49C4 0%, #BC3ED8 100%);
    padding: 32px 0;
    color: #fff;
}
.links_menu > a{
        padding: 12px 15px;
}
.links_menu > a:hover{
    opacity: 0.5;
}
.link_ativo{
    text-decoration: underline;
}

main{
    background-color: #f3f5f7;
    padding: 64px 0;
    min-height: 100vh;
}
.post{
    background-color: #fff;
    padding: 25px
}
.conteudo_post > h2{
    margin: 16px 0 5px
}
.cabecalho_post > p, .conteudo_post> p{
    color: #b6b6b6;
    font-weight: 400;
}
.cabecalho_post > i{
    color: #BC3ED8;
    font-size: 25px;
}
.cabecalho_post > i:hover::before{
    font-family: "Font Awesome 5 Free";
    content: "\f004";
    font-weight: 900;
    cursor: pointer;
}
.conteudo_post > h2{
    color: #313131;
    font-weight: 400;
}
