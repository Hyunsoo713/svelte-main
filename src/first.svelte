<script>


</script>

<main>
  
  <body>
    <div id="app">

      <div class="outline">  
          <span></span>
          <span></span>
          <span></span>
          <span></span>
          <a class='select-page' href="./date.html">
            <div id="title">Boxfolio</div>
          </a>
      </div>
    </div>
  </body>

</main>

<style>
body{

width: 100vw;
height: 100vh;
margin:auto 0;
padding:0;
}

#app{
width:100vw;
height:100vh;
display: flex;
align-items: center;
justify-content: center;
}

.outline{
position:relative;
width: 500px;
height:200px;
margin:30px auto;
border: 0px solid;
}
.outline span{position: absolute; background: darkblue;}

.outline span:nth-child(1) {left: 0; top: 0; width: 0; height: 2px; transition: width 0.1s;}
.outline span:nth-child(2) {right: 0; top: 0; width: 2px; height: 0; transition: height 0.1s linear 0.1s;}
.outline span:nth-child(3) {right: 0; bottom: 0; width: 0; height: 2px; transition: width 0.1s linear 0.2s;}
.outline span:nth-child(4) {left: 0; bottom: 0; width: 2px; height: 0; transition: height 0.1s linear 0.3s;}


.outline:hover span:nth-child(1) {width: 100%;}
.outline:hover span:nth-child(2) {height: 100%;}
.outline:hover span:nth-child(3) {width: 100%;}
.outline:hover span:nth-child(4) {height: 100%;}

.select-page{
text-decoration: none;
}

#title{
z-index: 1000px;
padding-top:40px;
padding-bottom:40px;
padding-left:20px;
padding-right:20px;
position: flex;
font-family: 'Raleway', sans-serif;
text-align: center;
font-size:120px;

background: linear-gradient(90deg,rgb(100,100,0), rgb(53, 73, 198));
color: transparent;
-webkit-background-clip: text;
background-clip: text;

}


#title:hover{
color:white;
background: rgb(118, 124, 10) ;
animation-name: ggs;
animation-duration: 3s;
}

@keyframes ggs{
0%{
  opacity: 0;
}
100%{
  opacity: 1;
}
}

a{
transition-delay: 2s;
}


</style>

