@import url("https://fonts.googleapis.com/css2?family=Barlow:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,100;0,9..144,200;0,9..144,300;0,9..144,400;0,9..144,500;0,9..144,600;0,9..144,700;0,9..144,800;0,9..144,900;1,9..144,100;1,9..144,200;1,9..144,300;1,9..144,400;1,9..144,500;1,9..144,600;1,9..144,700;1,9..144,800;1,9..144,900&display=swap");

/_ps: si jamais tu vois pourquoi mes animations finissent de manière si brut je suis preneur_/

/_Animation_/
@keyframes slide-bottom {
0% {
transform: translateY(0);
}
100% {
transform: translateY(100px);
}
}
@keyframes scale-animation {
0% {
transform: scale(1.2);
}
100% {
transform: scale(1);
}
}
/_parametre de base_/

- {
  margin: 0;
  padding: 0;
  text-decoration: none;
  box-sizing: border-box;
  list-style: none;
  overflow-x:hidden;
  }
  body{
  text-align: center;
  }
  .container {
  position: relative;
  width: 100vw;
  height: 100vh;
  font-family: 'Barlow', sans-serif;
  overflow-x:hidden;
  }
  h1{
  color: white;
  font-size: 11vw;
  font-family: 'Fraunces', serif;
  font-weight: 900;
  letter-spacing: 1vw;

}
h2{
color: #24303E;
font-size: 9vw;
font-family: 'Fraunces', serif;
font-weight: 900;
margin: 15vw 0 8vw 0;
}
h3{
font-size: 5vw;
font-family: 'Fraunces', serif;
color: hsl(210, 4%, 67%);
margin-top: 40vw;
letter-spacing: 1.5vw;
}
h4{
font-family: 'Fraunces', serif;
font-size: 5vw;
margin-top: 8vw;
}
h5{
font-family: 'Barlow', sans-serif;
color: #A7AAAD;
font-size: 4vw;
font-weight: 600;
margin-top: 4vw;
}
p{
margin: 0 10% 10%;
color: #808397;
font-weight: 600;
font-size: 4.5vw;
line-height: 7vw;
}
/_Header_/
header{
overflow: hidden;
.background{
width: 200vw;
height: 110vw;
margin-left: -49vw;
margin-top: -0.1vw;
}
h1{
position: absolute;
top: 35vw;
animation: scale-animation 1s ;  
 }
}
.logo {
width: 35vw;
height: 7vw;
margin: 6vw 0 0 5vw;
}
.menu {
position: absolute;
width:6vw;
height: 5vw;
top: 6.5vw;
left: 85vw;
}
.arrow{
position: absolute;
width:6vw;
height: 20vw;
top: 55vw;
left: 45vw;
animation: slide-bottom 1.5s forwards;
}
/_NAVBAR_/
.hamburger{
display: none;
}
nav {
display: flex;
background-color: #3ebfff;
padding-bottom: 30vw;
width: 100vw;
height: 8vw;
color:#24303E;
font-size: 4.5vw;
font-family: 'Fraunces', serif;
font-weight: 900;
ul{
color: #5B636D;
position: absolute;
background-color: hsl(0, 0%, 100%, 0.7);
width: 50vw;
height: 50vw;
right: 10vw;
top: 20vw;
z-index: 1;
font-weight: 600;
font-size: 3.5vw;
li{
margin-top: 6vw;
&:hover{
color: hsl(51, 100%, 49%);
transition: 0.2s;
}
}
}
}
.triangle{
display : flex;
position: absolute;
height : 0;
width : 0;
border-bottom : 7vw solid hsl(0, 0%, 100%, 0.7);
border-left : 7vw solid transparent;
top:13vw ;
right: 10vw;
}

.contact{
font-size: 3.5vw;
font-weight: 600;
background-color:hsl(51, 100%, 49%);
margin: 6vw 13vw;
padding: 2vw;
border-radius: 50px;
color: white;
&:hover{
outline: hsl(51, 100%, 49%) solid 0.4vw;
color: #5B636D;
background-color: transparent;
transition: 0.2s;
}
}

/_ Pas eu le temps d'apprendre a faire appaître avec js _/
header:hover{
.hamburger{
display: block;
}
}
/_parent1_/
.parent1 {
display: grid;
grid-template-columns: 100vw;
grid-template-rows: 80vw;
}

    .egg img{ grid-area: 1 / 1 / 2 / 2;
        width: 100vw;
        height: 85vw;
        margin-top: -1vw;
     }
    .text1 { grid-area: 2 / 1 / 3 / 2;
        margin-bottom: 15vw;
        margin-top: 1vw;

&:hover{
h2{
color:hsl(51, 100%, 49%);
opacity: 0.8;
transition: 0.3s;
}
}
}
a{
width: 100vw;
color:#5B636D;
font-size: 4.5vw;
font-family: 'Fraunces', serif;
font-weight: 900;
&:hover{
color: #24303E;
transition: 1s;
&::before{
opacity: 1;
transition: 1s;  
 }
}
&::before{
content: "";
width: 35vw;
height: 2vw;
background: hsl(51, 100%, 49%);
position: absolute;
border-radius: 50px;
z-index: -1;
opacity: 0.2;
transform: translateY(3.8vw) translateX(-1vw);
}
}

    .wine img{ grid-area: 3 / 1 / 4 / 2;
        width: 100vw;
        height: 85vw;}
    .text2 { grid-area: 4 / 1 / 5 / 2;
        margin-bottom: 15vw;
        &:hover{
            h2{
                color:hsl(7, 99%, 70%);
                opacity: 0.8;
                transition:  0.3s;
            }
        }
        a::before{background-color: hsl(7, 99%, 70%);}
    }

/_parent2_/

.parent2 {
display: grid;
grid-template-columns: 100vw;
grid-template-rows: 80vw;
p{
font-size: 3.7vw;
font-weight: 600;
line-height: 6vw;
margin-bottom: 15vw;
}
}

    .cherry {
        grid-area: 1 / 1 / 2 / 2;
        width: 192vw;
        margin: 0 0 -75vw -45vw ;}
    .cherrytext {
        grid-area: 2 / 1 / 3 / 2;
        p{
            color: hsl(167, 40%, 24%);
            font-weight: 600;
            line-height: 6vw;
            margin-bottom: 15vw;
           }
        h2{
            color: hsl(167, 40%, 24%);
            font-size: 8vw;
           }
           &:hover{
            p{
                color: white;
                transition: 0.6s;
            }
            h2{
                color: white;
                transition: 0.5s;
            }
        }
    }
    .orange{
        grid-area: 3 / 1 / 4 / 2;
        width: 192vw;
        height: 160vw;
        margin: 0 0 -75vw -45vw ;
    }
    .orangetext{
        grid-area: 4 / 1 / 5 / 2;
        p{
            color: hsl(198, 62%, 26%);
            font-size: 3.7vw;
            font-weight: 600;
            line-height: 6vw;
            margin-bottom: 15vw;
        }
           h2{
            color: hsl(198, 62%, 26%);
            font-size: 8vw;}
            &:hover{
                p{
                    color: white;
                    transition: 0.6s;
                }
                h2{
                    color: white;
                    transition: 0.5s;
                }
            }
     }

/_Testimonials _/
.testimonials{
img{
margin-top: 20vw;
width: 20vw;
border-radius: 50%;
}
p{
font-size: 4.4vw;
color: #5B636D;
margin-top: 8vw;
}
h3{
margin-top: 30vw;

    }

}
/_Grid avec 4 images carré_/
.parent3{
display: grid;
grid-template-columns: repeat(2, 1fr);
grid-template-rows: repeat(2, 1fr);
margin: 25vw 0 -15vw 0;

        .milk { grid-area: 1 / 1 / 2 / 2;
            width: 50vw;
            height: 50vw;}
        .fruit{
            grid-area: 1 / 2 / 2 / 3;
            width: 50vw;
            height: 50vw;
        }
        .cone {
            grid-area: 2 / 1 / 3 / 2;
            width: 50vw;
            height: 50vw;}
        .sugar {
            grid-area: 2 / 2 / 3 / 3;
            width: 50vw;
            height: 50vw;}
    }
    /*Footer + logo + liens vers les réseau sociaux*/

footer{
background-color:#90D4C6 ;
h2{
padding-top: 12vw;
font-size: 8vw;
font-family: 'Barlow', sans-serif;
color: #2C7566;
font-weight:800;
}
ul{
display: flex;
flex-direction: row;
justify-content: space-around;
font-size: 4vw;
font-weight: 500;
color:#2C7566 ;
margin: 10vw 0 5vw 0;
:hover{
color: white;
transition: 0.2s;
}
}
.social{
display: flex;
justify-content: center;
padding: 15vw 0;
margin: 2vw 25vw;
img{
width: 4.5vw;
margin: 0 5vw;
}
}
}

/_ Desktop configuration j'ai préféré mettre une résolution qui peut fonctionner sur tablette aussi car je trouve ca plus joli le format desktop sur une tablette que le format mobile _/
@media screen and (min-width : 768px){  
main{
width: 100vw;
height: 100vh;
text-align: left;
}
/_header_/
header {
.logo{
position: absolute;
width: 18vw;
height: 4vw;
top:-2vw;
left: 0vw;
}
.menu{
display: none;
}
.arrow{
width: 3vw;
height: 10vw;
top: 24vw;
left: 48vw;
}
.background {  
 opacity: 1;
margin-left: 0;
width: 100vw;
height: auto;
}
h1{
width: 100vw;
font-size: 5vw;
top: 20vw;
text-align: center;
}  
 nav{
padding-bottom: 3vw;
ul{
display: flex;
color: white;
position: relative;
background-color: transparent;
margin-left: 70vw;
width: 50vw;
height: auto;  
 font-weight: 400;
font-size:1.6vw;
margin-top: -21.5vw;
li{
margin-right: 3vw;
}
}
}
.contact{
color:#5B636D;
background-color: hsl(0, 0%, 100%);
font-size: 1.3vw;
padding: 1vw;
margin-top: 5.3vw;
margin-left: -1vw;
&:hover{
color: white;
background-color: hsl(0, 0%, 100%, 0.3);
outline: none;
}
}
.triangle{
display: none;
}
}
.hamburger{
display: block;
}
/_parent1_/
.parent1 {
grid-template-columns: 50vw;
grid-template-rows: 45vw;

    .egg img { grid-area: 1 / 2 / 2 / 3;
        width: 50vw;
        height: 45vw;
        margin-top: -0.2vw;
     }
    .text1 { grid-area: 1 / 1 / 2 / 2; ;
        margin-left: 8vw;
        margin-right: 2vw;
            h2{
                font-size: 3.7vw;
                text-align: left;
                margin-top: 8vw;
                margin-bottom: 2vw;
             }
            p{
                 font-size: 1.4vw;
                 line-height: 3vw;
                 font-weight: 500;
                 text-align: left;
                 margin-left: 0;
            }
            a{
                font-size: 1.3vw;
                margin-top: -5vw;
                &:hover{
                    color:   #24303E;
                    transition: 1s;
                    &::before{
                        opacity: 1;
                        transition: 1s;
                    }
                }
                &::before{
                    content: "";
                    width: 11vw;
                    height: 1vw;
                    background: hsl(51, 100%, 49%);
                    opacity: 0.2;
                   transform: translateY(1vw) translateX(-0.9vw);
                }
            }
        }
    .wine img{grid-area: 2 / 2 / 3 / 3;
        width: 50vw;
        height: 45vw;
        margin-top: -0.2vw;
    }
    .text2 {
        grid-area: 2 / 2 / 3 / 3;;
            margin-left: 8vw;

            h2{
                font-size: 3.7vw;
                text-align: left;
                margin-top: 8vw;
                margin-bottom: 2vw;
             }
            p{
                 font-size: 1.4vw;
                 line-height: 3vw;
                 font-weight: 500;
                 text-align: left;
                 margin-left: 0;
            }
            a{
                font-size: 1.3vw;
                margin-top: -5vw;
                &:hover{
                    color:   #24303E;
                    transition: 1s;
                    &::before{
                        opacity: 1;
                        transition: 1s;
                    }
                }
                &::before{
                    content: "";
                    width: 11vw;
                    height: 1vw;
                    opacity: 0.2;
                    transform: translateY(1vw) translateX(-0.9vw);
                }
            }
    }

}  
 /_parent2_/
.parent2 {
grid-template-columns: 50vw;
grid-template-rows: 45vw;
margin-top: -10vw;
text-align: center;

        h2{ font-size: 2.2vw;
            margin-bottom: 3vw;

        }
        p{
            font-size: 1.4vw;
            line-height: 2vw;
            margin: 0 20%;
            font-weight: 500;
        }

        .cherry {
            grid-area: 1 / 1 / 2 / 2;
            width: 50vw;
            height: 45vw;
            margin-left: 0;
         }
        .orange {
            grid-area: 1 / 2 / 2 / 3;
            width: 50vw;
            height: 45vw;
            margin-left: 0;
         }
        .cherrytext{
            grid-area: 2 / 1 / 3 / 2;
            width: 50vw;
            height: 45vw;
            margin-top: -32vw;

        }
        .orangetext {
            grid-area: 2 / 2 / 3 / 3;
            width: 50vw;
            height: 45vw;
            margin-top: -32vw;

    }

}
/_parent2_/
.testimonials{
h3{
font-size: 1.7vw;
text-align: center;
margin-top: 0vw;
letter-spacing: 1vw;
}
}
.parent3 {
display: grid;
grid-template-columns: 35 30 35vw;
grid-template-rows: 1fr;
text-align: center;
margin-top: -10vw;
p{
font-size: 1.5vw;
line-height: 2vw;
margin: 0 5%;
font-weight: 500;
}
img{
width: 6vw;
margin-bottom: 5vw;
}
h4{
font-size: 1.9vw;

    }
    h5{
        font-size: 1.5vw;
        margin-top: 1vw;
    }
    .emily {
        grid-area: 1 / 1 / 2 / 2;
        width: 33vw;

}
.thomas {
grid-area: 1 / 2 / 2 / 3;
width: 33vw; }
.jennie {
grid-area: 1 / 3 / 2 / 4;
width: 33vw; }
}
.parent3 {
display: grid;
grid-template-columns: 25vw;
grid-template-rows: 1fr;
margin-top: 10vw;

        .milk{
            grid-area: 1 / 1 / 2 / 2;
            width: 25vw;
            height: auto;
        }
        .fruit{
            grid-area: 1 / 2 / 2 / 3;
            width: 25vw;
            height: auto;
         }
        .cone {
            grid-area: 1 / 3 / 2 / 4;
            width: 25vw;
            height: auto;
        }
        .sugar {
            grid-area: 1 / 4 / 2 / 5;
            width: 25vw;
            height: auto;
         }

}
footer{
h2{
text-align: center;
font-size: 2.3vw;
margin-top: 7vw;
margin-bottom: 8vw;
}
ul{
margin: -5vw 35vw 0;
}
li{
font-size: 1.5vw;
}
.social{
padding: 0;
margin: 2vw 40vw 0vw 40vw;
padding-bottom: 5vw;
img{
margin: 0 1vw;
width:1.5vw;
}  
 }
}
}
