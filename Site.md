# Site para um evento.


HTML para o Site do Evento.

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Evento Importante </title>
    
    <!--Estilos-->
    <link rel="stylesheet" href="css/styles.CSS">
    <!--Estilos-->

    <!--Google fonts-->
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&family=VT323&display=swap" rel="stylesheet">
    <!--Google fonts-->

</head>


<body>
   <div id="about-container">
    <div id="brand">
        <img src="img/saasweeklogo.png" alt="SaaS Week">
        <h1>SaaS Week</h1>
    </div>
    <p id="exclusive">Webinar Exclusivo</p>
    <h2>Aprenda a criar um software para gerar renda</h2>
    <p id="date">29/10/2022 | 14h00 | 100% Gratuito</p>
    <p id="description">Neste evento você aprenderá a planejar um software SaaS. E também a como comercializar o produto que você desenvolveu.</p>
    <h4>Palestrantes</h4>
    <div id="users-container">
        <div class="user-card">
            <img src="img/user_1.jpg" alt="Paul Smith">
            <p class="user-name">Paul Smith</p>
            <p class="user-role">Gerente de Marketing</p>
        </div>
        <div class="user-card">
            <img src="img/user_2.jpg" alt="Jon Doe">
            <p class="user-name">Jon Doe</p>
            <p class="user-role">Tech Lead</p>
        </div>
        <div class="user-card">
            <img src="img/user_3.jpg" alt="Brad Young">
            <p class="user-name">Brad Young</p>
            <p class="user-role">Empreendedor</p>
        </div>
    </div>

   </div>
   

   <div id="form-container">
    <div id="form-inner">
        <h3>Se inscreva</h3>
        <p>Não perca a oportunidade de aprender com especialistas e tirar suas dúvidas.</p>
        <form id="register-form">
            <div id="name-container">
                <input type="text" name="name" id="name" placeholder="Nome">
                <input type="text" name="lastname" id="lastname" placeholder="Sobrenome">
            </div>
            <input type="email" name="email" id="email" placeholder="Digite seu e-mail"> <br>
            <input type="submit" value="Cadastrar" >
            </form>
            <div id="benefits">
                <h4>O que você vai aprender?</h4>
                <ul>
                   <li>Como escolher uma stack de tecnologias</li>
                   <li>Criar um projeto SaaS</li>
                   <li>Prospectar Clientes</li>
                   <li>Estratégias de vendas</li>
                </ul>
            </div>
    </div>

   </div>
    
</body>
</html>



CSS para o Site do Evento.

/* Geral */
*{
    margin:0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Roboto";
}

body{
    display: flex;
    flex-wrap: wrap;
}

/* Apresentação do Evento */
#about-container{
    flex: 1.4;
    padding: 2rem 4rem;
}

#brand {
    display: flex;
    align-items: center;
    font-size: 0.8rem;
    margin-bottom: 1rem;
}

#brand img {
    height: 50px;
    margin-right: 0.6rem;
}

#exclusive {
    text-transform: uppercase;
    color: #0075ff;
    font-weight: bold;
    font-size: 0.9rem;
    margin-bottom: 1rem;
}

#about-container h2 {
    font-size: 2.4rem;
    max-width: 500px;
    margin-bottom: 1rem;
}

#date {
    text-transform: uppercase;
    color: #aaa;
    margin: 1rem;
}

#description {
    max-width: 500px;
    margin-bottom: 1rem;
    line-height: 1.4rem;
}

#about-container h4 {
    font-size: 1.4rem;
    margin-bottom: 1rem;
}

#users-container {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
}

.user-card {
    border: 2px solid #ccc;
    padding: 1rem;
    width: 180px;
    text-align: center;
}

.user-card img {
    width: 120px;
    border-radius: 50%;
    margin-bottom: 1rem;
}

.user-card .user-name {
    font-weight: bold;
    margin-bottom: 0.6rem;
}

.user-card .user-role {
    color: #aaa;
    font-size: 0.9rem;
}

/* Formulário */
#form-container {
    flex: 1;
    background-image: url("../img/pattern.png");
    background-size: cover;
    color: #fff;
}

#form-inner {
    margin: 3rem;
    padding: 3rem;
    border: 2px solid #fff;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
}

#form-inner h3 {
    font-size: 2rem;
    margin-bottom: 1rem;

}

#form-inner p {
    margin-bottom: 1rem;
}

#register-form {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
    margin-bottom: 2rem;
}

#name-container {
    display: flex;
    gap: 0.5rem;
}

#register-form input {
    padding: 0.8rem 0.6rem;
    border: none;
    border-radius: 3px;
}

#email {
    min-width: 100%;
}

#register-form input[type="submit"]{
    background-color: transparent;
    color: #fff;
    border: 2px solid #fff;
    font-size: 1.1rem;
    font-weight: bold;
    cursor: pointer;
    transition: 0.4s;

}

#register-form input[type="submit"]:hover{
    background-color: #fff;
    color: #0075ff;
}

#benefits {
    text-align: left;
    
    
}

#benefits h4 {
    font-size: 1.4rem;
    margin-bottom: 1rem;

}

#benefits ul {
    list-style-position: inside;
}

#benefits li {
    margin-bottom: 0.5rem;

}

/* Responsivo */ 

@media (max-width: 450px){
    body{
        flex-direction: column;

    }
    #about-container {
        padding: 2rem;
        padding-bottom: 0;

    }
    #about-container h2 {
        font-size: 3rem;
    }

    #exclusive, #date {
        font-size: 1.4rem;
    }
    #description {
        font-size: 1.6rem;
        line-height: 2.2rem;

    }

    #users-container {
        flex-direction: column;
    }

    .user-card {
        width: 100%;
        padding: 2rem;
    }

    #user-card img {
        width: 180px;

    }

    .user-card .user-name {
        font-size: 1.6rem;
    }

    .user-card .user-role {
        font-size: 1.4rem;
    }

    #form-inner {
        padding: 2rem;
        margin: 2rem;

    }

    #register-form, #name-container {
        gap: 1rem;
    }
}
