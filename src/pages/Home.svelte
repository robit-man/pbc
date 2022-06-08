<script>
import { onMount } from "svelte";
import { slide, fade } from 'svelte/transition';
import { Router, Link, Route } from "svelte-routing";

</script>

<main>
  <div class="wrapper">
<div class="row rotated" style="  ">
    <div class="arrow" style="position:absolute;top:-3rem;left:-3rem;height:4rem;width:4rem;box-shadow: -1.5rem -1.5rem #ff8f00;"></div>
    <div class="arrow" style="position:absolute;top:-6rem;left:-6rem;height:4rem;width:4rem;box-shadow: -1.5rem -1.5rem #ff8f00;"></div>
    <div class="arrow" style="position:absolute;top:-9rem;left:-9rem;height:4rem;width:4rem;box-shadow: -1.5rem -1.5rem #ff8f00;"></div>
      <header>


        
      <svg class="hov" version="1.0" xmlns="http://www.w3.org/2000/svg" style=""
      width="200.000000px" height="200.000000px" viewBox="0 0 400.000000 400.000000"
      preserveAspectRatio="xMidYMid meet">
     
      <g style="animation-duration: 3s;" fill="white" stroke="none" transform="translate(-800.000000,400.000000) scale(0.100000,-0.100000)">
     
     <path d="M8090 2000 l0 -2000 1995 0 1995 0 0 985 0 985 -1005 0 -1005 0 0 30
     0 30 1005 0 1005 0 0 985 0 985 -1995 0 -2000 0 0 -2000z"/>
                
     </g>
     </svg>


     <svg class="hov" version="1.0" xmlns="http://www.w3.org/2000/svg" style="animation-duration: 7s;"
     width="200.000000px" height="200.000000px" viewBox="0 0 400.000000 400.000000"
     preserveAspectRatio="xMidYMid meet">
    
     <g transform="translate(-400.000000,400.000000) scale(0.100000,-0.100000)"
    fill="white" stroke="none">
    <path d="M4050 2000 l0 -2000 1990 0 1990 0 0 2000 0 2000 -1990 0 -1990 0 0
    -2000z m3020 1000 l0 -30 -1030 0 -1030 0 0 30 0 30 1030 0 1030 0 0 -30z m0
    -2000 l0 -30 -1030 0 -1030 0 0 30 0 30 1030 0 1030 0 0 -30z"/>
    </g>
    </svg>   
    

    <svg class="hov" version="1.0"  xmlns="http://www.w3.org/2000/svg" style="animation-duration: 10s;"
    width="200.000000px" height="200.000000px" viewBox="0 0 400.000000 400.000000"
    preserveAspectRatio="xMidYMid meet">

    <g style="animation-duration: 6s;" transform="translate(0.000000,400.000000) scale(0.100000,-0.100000)"
    fill="white" stroke="none">
    <path d="M0 2000 l0 -2000 995 0 995 0 0 1005 0 1005 1000 0 1000 0 0 995 0
    995 -1995 0 -1995 0 0 -2000z m3030 1000 l0 -30 -1030 0 -1030 0 0 30 0 30
    1030 0 1030 0 0 -30z"/>
    <path d="M2050 975 l0 -975 970 0 970 0 0 975 0 975 -970 0 -970 0 0 -975z"/>

    </g>
    </svg>    

      

             </header>
      <article> 
      
      
        <div class="line" style="display:flex;flex-flow:wrap;justify-content:center;"><img class="imgspin" src="/imgs/pointblank.svg" alt=""></div>
 
          <div>
          <p >
              <b transition:fade  style="color:#ff8f00;" >POINTBLANK LLC</b> is a Rapid Prototyping, Aerospace, and DAPP Development public benefit corporation out of Portland Oregon
            </p> 
            </div>


            <div class="button-row">
                <a href="https://www.prnewswire.com/news-releases/spacex-to-launch-doge-1-to-the-moon-301287016.html"><button>DOGE-1</button></a><div class="crosshair" style="margin-left:0.3rem;"></div>
                <a href="https://xiprotocol.io/"><button>XI PROTOCOL</button></a>
                <a href="https://noclip.org/"><button>NOCLIP</button></a>
                <a href="https://revest.finance/"><button>REVEST</button></a><div class="crosshair" style="margin-left:0.3rem;"></div>
                <a href="https://rena.finance"><button>RENA</button></a>
                <a href="https://www.olympusdao.finance/"><button>OLYMPUS</button></a>
                <a href="https://www.guranft.com/"><button>GURA NFT</button></a>        <div class="crosshair" style="margin-left:0.3rem;"></div>
                <a href="https://twitter.com/POINTBLANK_LLC" > <button>TWITTER</button> </a>
              </div>    
    </article>
</div>
    
    <!--
    <footer transition:slide >
        <div class="row">
        <div class="column">
            <p style="font-size:10px;max-width:128px;">Inquiries will be selected and responses given at our discretion.</p>
            <a href="https://pointblank.company/contact"><button>CONTACT</button></a>
        </div>
        <img class="footer-arrow" src="/imgs/fast-forward.svg" alt="">
        </div>

    </footer>-->
  </div>
</main>

<style>
.wrapper{
    padding:0rem;
    margin: auto;
    height:100vh;display:flex;justify-content: center;
    overflow-x: hidden;
}
@keyframes slide{
    0%{background-position-x: 0rem;background-position-y: 0rem;}
    20%{background-position-y: -2rem;background-size:1rem;background-position-x: 2rem;}
    30%{background-position-y: -1rem;background-position-x: 0rem;}
    50%{background-position-x: 2rem;background-position-y: -3rem;}
    60%{background-position-x: 0rem;background-size:4rem;background-position-y: 0rem;}
    70%{background-position-y: 2rem;background-position-x: 1rem;}
    90%{background-position-y: -2rem;background-position-x: 0rem;}
    100%{background-position-x: -2rem;background-size:1rem;background-position-y: 4rem;}
}
header > svg{transform:rotate(-90deg)}
header{
    height:600px;
    background: black;
  width: min-content;
  padding: 1.5rem;
  display: flex;
  flex-flow: wrap;
  justify-content: center;
  pointer-events: none;
}
header > h1{
    text-align:left;
    margin-top:auto;
    margin-right:auto;
    margin-left:0.5rem;
    margin-bottom: unset;
    font-size:6rem;
    line-height: 0.8;   
}
header > img{width: 1024px;
height: 339px;
height: inherit;
transform: rotate(90deg);

}
@keyframes glitch2{
    0%{fill:white;}
    20%{fill:white;}
    21%{fill:#ff8f00;}
    22%{fill:white;}
    42%{fill:white;}
    43%{fill:#ff8f00;}
    47%{fill:white;}
    48%{fill:#ff8f00;}
    60%{fill:white;}
    78%{fill:white;}
    72%{fill:#ff8f00;}
    75%{fill:white;}
    100%{fill:white;}
}

@keyframes glitch{
    0%{opacity: 1;}
    20%{opacity: 1;}
    21%{opacity: 0;}
    22%{opacity: 1;}
    52%{opacity: 1;}
    53%{opacity: 0;}
    57%{opacity: 1;}
    58%{opacity: 0;}
    60%{opacity: 1;}
    88%{opacity: 1;}
    92%{opacity: 0;}
    95%{opacity: 1;}
    100%{opacity: 1;}
}
@keyframes spread{
    0%{box-shadow:0rem 0rem #ff8f00,0rem -24rem #2d2d2d,-24rem 0rem #1e1e1e,0rem 0rem #4d4d4d;}
    20%{box-shadow:-1.5rem 0rem #ff8f00,0rem -24rem #2d2d2d,-24rem 0rem #1e1e1e,0rem 0rem #4d4d4d;}
    40%{box-shadow:-1.5rem -1.5rem #ff8f00,0rem -24rem #2d2d2d,-24rem 0rem #1e1e1e,0rem 0rem #4d4d4d;}
    60%{box-shadow:-1.5rem -1.5rem #ff8f00,0px -24px #2d2d2d,-24px 648px #1e1e1e,0rem 648px #4d4d4d;}
    80%{box-shadow:-1.5rem -1.5rem #ff8f00,648px -24px #2d2d2d,-24px 648px #1e1e1e,648px 648px #4d4d4d;}
    100%{box-shadow:-1.5rem -1.5rem #ff8f00,648px -24px #2d2d2d,-24px 648px #1e1e1e,648px 648px #4d4d4d;}
}
.hov{animation:glitch 4s linear infinite;}
.hov > g{animation:glitch2 5s linear infinite;}
.imgspin{animation:spin 10s linear infinite;height: calc(100% - 1rem);
margin: auto;
padding: 0.5rem;
mix-blend-mode: exclusion;
border-radius: 100%;
filter: invert(1);}
.rotated{animation:spread 1s ease;transition:all 0.5s ease;box-shadow:-1.5rem -1.5rem #ff8f00,648px -24px #2d2d2d,-24px 648px #1e1e1e,648px 648px #4d4d4d;
flex-flow:row-reverse;transform:rotate(45deg);margin:auto;transition:all 0.2s ease;}
.line{transform:rotate(-45deg);filter:invert(1);
max-height: 300px;clip-path: polygon(0 0, 100% 0%, 100% 0rem, 100% 100%, 4rem 100%, 0 calc(100% - 4em));
   background-image:url(/imgs/hqr.gif), url(/imgs/lqr.gif), radial-gradient(transparent,transparent, transparent, white, white, white);background-blend-mode:color-dodge;background-size:cover;mix-blend-mode: color;background-position:center;background-repeat: no-repeat;
    background-color:transparent;height:calc(100% - 3rem);width:calc(100% - 3rem);margin: 1.5rem;border-radius: 100%;
margin-top: 1.3rem;}
footer{
    margin-top: 2rem;
    padding: 2rem;
    border: 10px solid;
    border-image-slice: 1;
    border-width: 5px;    
    width: max-content; 
    border-image-source: linear-gradient(to left, black, black, white);
}
footer > .row p{
    color:white;
    text-align:left;
    margin-top:-4px;
}
article{
    padding:0.5rem 0rem;display:flex;flex-flow:wrap;justify-content:space-between;max-width:400px;
    margin-top:1rem;height:600px;
}
article > div > p{line-height: 1.1;letter-spacing: 0.3rem;
    text-align: right;text-transform:uppercase;font-size:1.3rem;
   
    color:rgb(255, 255, 255);margin:unset;
margin-bottom: unset !important;
margin-right:-0.3rem;
}
.row{display:flex;flex-flow:row-reverse;}
.column{display:flex;flex-flow:column;}
.button-row{
    display: flex;
    flex-flow: wrap;
    justify-content: flex-end;max-width: 600px;padding-top:1rem;
height: fit-content;
margin-top: -0.2rem;
}.crosshair{background-image:url(/imgs/crosshair.svg); width:2.32rem;height:2.32rem;background-size:2.32rem;filter:invert(1);transition:all 0.2s ease;}.crosshair:hover{clip-path: polygon(0 0, calc(100% - 1rem) 0%, 100% 1rem, 100% 100%, 1rem 100%, 0 calc(100% - 1rem));}
.footer-arrow{
    filter: invert(1);
    margin-left: 2rem;
    height: 145px;
    margin-top: -20px;
    margin-bottom: -20px;
}
button img{
    filter: invert(1);
height: 34px;
margin-bottom: -14px;
margin-top: -8px;
transition:filter 200ms ease;
}
button:hover img{
    filter:invert(0);
}
.button-row > a {margin-left:0.3rem;
margin-bottom:0.3rem;}
@keyframes spin {
    0%{transform:rotate(0deg);
    }
    100%{transform:rotate(360deg);
    }
}
@media screen and (max-width: 1000px){
header > h1{
    margin-left:0rem;
    line-height: 1;   
    font-size:2rem;
    line-height:0.7;


}    .arrow{display:none;}

.wrapper{height:calc(100vh - 2rem);padding:1rem;}

header > svg{transform:rotate(0deg);width:33%;height:auto;}

.rotated{box-shadow: 1.5rem 0rem #ff8f00;
border-top-left-radius: 0rem;display:flex;flex-flow:column;transform:rotate(0deg);margin:auto;transition:all 0.2s ease;padding-right:1rem;}
.line{transform:rotate(0deg);height:300px;clip-path: polygon(0 0, 100% 0%, 100% 0rem, 100% 100%, 2rem 100%, 0 calc(100% - 2rem));}
article{max-width:600px;height:auto;width:100%;flex-flow:wrap;margin-bottom: -0.7rem;}
    header{
    height:auto;
    width: 100%;
    padding:0rem;
    display: flex;
    flex-flow: row-reverse;
    justify-content: space-between;
    clip-path: unset;
    pointer-events: none;
    border-top-right-radius: unset;
    margin-top: 0rem;
    }
}
@media screen and (max-height: 950px){
    .arrow{display:none;}
header > h1{
    margin-left:0rem;
    line-height: 1;   
    font-size:2rem;
    line-height:0.7;


}
.wrapper{height:calc(100vh - 2rem);padding:1rem;}

header > svg{transform:rotate(0deg);width:33%;height:auto;}

.rotated{box-shadow: 1.5rem 0rem #ff8f00;
border-top-left-radius: 0rem;display:flex;flex-flow:column;transform:rotate(0deg);margin:auto;transition:all 0.2s ease;padding-right:1rem;}
.line{transform:rotate(0deg);height:300px;clip-path: polygon(0 0, 100% 0%, 100% 0rem, 100% 100%, 2rem 100%, 0 calc(100% - 2rem));}
article{height:auto;width:100%;flex-flow:wrap;max-width:600px;margin-bottom: -0.7rem;}
    header{
    height:auto;
    width: 100%;
    padding:0rem;
    display: flex;
    flex-flow: row-reverse;
    justify-content: space-between;
    clip-path: unset;
    pointer-events: none;
    border-top-right-radius: unset;
    margin-top: 0rem;
    }
}

</style>
