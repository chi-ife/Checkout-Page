@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');

*{
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}

body{
    font-family: 'Lato', sans-serif;
    background-image: url(./images/body-bg.png);
    background-repeat: no-repeat;
    background-size: 100%;
}

main{
   
    margin: 50px 170px;
    display: flex;
    flex-flow: row;
    height: 700px;
}

.credit-card-info{
    background: #89ace3c2;
    background-image: url(./images/main-bg.png);
    background-size: cover;
    background-repeat: no-repeat;
    justify-content: flex-start;
    height: 100%;
    padding: 100px 0 60px 50px;
    border-radius: 32px 0 0 32px;
    display: flex;
    flex-flow: column;
    gap: 25px;
    color: #fff;
    flex-basis: 60%;
}

.credit-card-links{
    border-bottom: 0.5px solid rgba(255, 255, 255, 0.445);
    display: flex;
    gap: 30px;
    width: 200px;
}

.credit-card-links a{
    text-decoration: none;
    font-weight: 600;
    color: #fff;
}

.cred-card{
    border-bottom: 2px solid #fff;
    
}

.img{
    transform: scale(0.7) translateX(-20%);
    margin-bottom: -20px;
}

.card-info{
    display: flex;
    flex-flow: column;
    gap: 15px;
    width: 600px;
}

.c-info-label{
    font-size: 12px;
    color: #fff;
    opacity: 0.7;
    
}

.top-part{
    display: flex;
    flex-flow: column;
    gap: 20px;
    width: 300px;
}

.inputs{
    border: 0;
    background-color: rgba(255, 255, 255, 0);
    border-bottom: 1px solid #fff;
    font-size: 16px;
    height: 30px;
    color: #fff;
}



.inputs::placeholder{
    color: #fff;
    padding: 0 0 0 10px;
    font-family: 'Lato';
    font-size: 17px;
}

.date-cvv{
    display: flex;
    flex-flow: row wrap;
    gap: 80px;
}

.date{
    display: flex;
    flex-direction: column;
    gap: 20px;
    width: 25%;
}

.cvv{
    display: flex;
    flex-direction: column;
    gap: 20px;
    margin-top: -14px;
    width: 15%;
}

.cvv img{
    transform: scale(0.8) translateY(32%);
    margin-left: 0px;
}

input[type=submit]{
    width: 250px;
    height: 35px;
    background: #fcf6f5;
    border: 0;
    color:#4986E0F2;
    font-size: 22px;
    padding: 7px 20px;
    border-radius: 13px;
    font-weight: 600;
    margin: 50px;

}

input[type=submit]:hover{
    cursor: pointer;
    background-color: #4986E0;
    color: #fff;
    border: 2px solid #fff;
    padding: 5px 10px;
}

.details{
    background: #FCF6F5;
    border-radius: 0 32px 32px 0;
    color: #4986E0;
    flex-basis: 40%;
}

.details .back-btn{
    transform: scale(0.8) translate(310px);  
}

.details-content{
    display: flex;
    flex-direction: column;
    margin-top: 30px;
}

.details-content .logo{
    transform: scale(0.5) translateY(-30%);

}

.details-content h2{
    align-self: center;
}

.details-content h4{
    align-self: center;
    margin-top: -110px;
    font-size: 22px;
    transform: translateY(30px);
}

em{
    font-size: 40px;
    margin-top: 70px;
    align-self: center;
    font-weight: 600;
}

.features{
     margin-top: 40px;
     align-self: center;
}

.feature{
    display: flex;
    flex-direction: row;
    gap: 20px;
    margin-bottom: 30px;
}

.feature img{
    transform: scale(0.8);
}

@media(max-width: 700px) {
    body{
        background-image: none;
    }
    
    main{
        display: grid;
        grid-template-areas: 
                'details'
                'card-info';   
        gap: -90px; 
        width: 100%;
        transform: translateX(-45%) translateY(-5%); 
    }
    section{
        display: block;
    }
    
    .credit-card-info{
        grid-area: card-info;
        background-image: url(./images/main-bg.png);
        width: 100%;
        border-radius: 0 0 32px 32px;
    }

    .details{
        grid-area: details;
        border-radius: 32px 32px 0 0;   
    }

    .details .back-btn{
        transform: translateX(320px) translateY(20px);
    }

    .card-info{
        width: 100%;
    }

    .date-cvv{
        width: 100%;
    }
    input[type=submit]{
        transform: translateX(-20%);
    }
    



}
  













