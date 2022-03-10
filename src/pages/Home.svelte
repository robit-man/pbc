<script>
import { onMount } from "svelte";
import { slide, fade } from 'svelte/transition';
import { Router, Link, Route } from "svelte-routing";

</script>

<main>
  <div class="wrapper">
<div class="row rotated">
      <header>


        
      <svg version="1.0" xmlns="http://www.w3.org/2000/svg" style=""
      width="200.000000px" height="200.000000px" viewBox="0 0 400.000000 400.000000"
      preserveAspectRatio="xMidYMid meet">
     
      <g fill="white" stroke="none" transform="translate(-800.000000,400.000000) scale(0.100000,-0.100000)">
     
     <path d="M8090 2000 l0 -2000 1995 0 1995 0 0 985 0 985 -1005 0 -1005 0 0 30
     0 30 1005 0 1005 0 0 985 0 985 -1995 0 -2000 0 0 -2000z"/>
                
     </g>
     </svg>


     <svg version="1.0" xmlns="http://www.w3.org/2000/svg" style=""
     width="200.000000px" height="200.000000px" viewBox="0 0 400.000000 400.000000"
     preserveAspectRatio="xMidYMid meet">
    
     <g transform="translate(-400.000000,400.000000) scale(0.100000,-0.100000)"
    fill="white" stroke="none">
    <path d="M4050 2000 l0 -2000 1990 0 1990 0 0 2000 0 2000 -1990 0 -1990 0 0
    -2000z m3020 1000 l0 -30 -1030 0 -1030 0 0 30 0 30 1030 0 1030 0 0 -30z m0
    -2000 l0 -30 -1030 0 -1030 0 0 30 0 30 1030 0 1030 0 0 -30z"/>
    </g>
    </svg>   
    

    <svg version="1.0"  xmlns="http://www.w3.org/2000/svg" style=""
    width="200.000000px" height="200.000000px" viewBox="0 0 400.000000 400.000000"
    preserveAspectRatio="xMidYMid meet">

    <g transform="translate(0.000000,400.000000) scale(0.100000,-0.100000)"
    fill="white" stroke="none">
    <path d="M0 2000 l0 -2000 995 0 995 0 0 1005 0 1005 1000 0 1000 0 0 995 0
    995 -1995 0 -1995 0 0 -2000z m3030 1000 l0 -30 -1030 0 -1030 0 0 30 0 30
    1030 0 1030 0 0 -30z"/>
    <path d="M2050 975 l0 -975 970 0 970 0 0 975 0 975 -970 0 -970 0 0 -975z"/>

    </g>
    </svg>    

      

             </header>
      <article> <div class="button-row">
        <a href="https://www.prnewswire.com/news-releases/spacex-to-launch-doge-1-to-the-moon-301287016.html"><button>DOGE-1</button></a><div class="crosshair" style="margin-left:0.3rem;"></div>
        <a href="https://xiprotocol.io/"><button>XI PROTOCOL</button></a>
        <a href="https://noclip.org/"><button>NOCLIP</button></a>
        <a href="https://revest.finance/"><button>REVEST</button></a><div class="crosshair" style="margin-left:0.3rem;"></div>
        <a href="https://rena.finance"><button>RENA</button></a>
        <a href="https://www.olympusdao.finance/"><button>OLYMPUS</button></a>
        <a href="https://www.guranft.com/"><button>GURA NFT</button></a>        <div class="crosshair" style="margin-left:0.3rem;"></div>

      </div>                    <div class="line" style=""></div>
 
          <div>
          <p >
              <b transition:fade  style="" >POINTBLANK LLC</b> is a Rapid Prototyping, Consulting, and App Development public benefit corporation out of Portland Oregon.
            </p> 
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
    0%{background-position-x: 0rem;}
    100%{background-position-x: 2rem;}
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
.rotated{transform:rotate(45deg);margin:auto;transition:all 0.2s ease;}
.line{clip-path: polygon(0 0, 100% 0%, 100% 0rem, 100% 100%, 4rem 100%, 0 calc(100% - 4em));
    animation:slide 1s linear infinite;background-image:url(/imgs/repeatline.svg);background-size:1rem;
    background-color:white;height:100%;width:100%;margin-bottom: 1.5rem;
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
    padding:0.5rem 0rem;display:flex;flex-flow:column;justify-content:space-between;max-width:400px;
    margin-top:1rem;height:600px;
}
article > div > p{line-height: 1.1;letter-spacing: 0.3rem;
    text-align: right;text-transform:uppercase;font-size:1.3rem;
   
    color:rgb(255, 255, 255);margin:unset;
margin-bottom: unset !important;
margin-right:-0.3rem;
}
.row{display:flex;flex-flow:row;}
.column{display:flex;flex-flow:column;}
.button-row{
    display: flex;
    flex-flow: wrap;
    justify-content: flex-end;max-width: 512px;
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


}
.wrapper{padding:1rem;}

header > svg{transform:rotate(0deg);width:auto;height:auto;}

.rotated{display:flex;flex-flow:column;transform:rotate(0deg);margin:auto;transition:all 0.2s ease;}
.line{height:100px;clip-path: polygon(0 0, 100% 0%, 100% 0rem, 100% 100%, 2rem 100%, 0 calc(100% - 2rem));}
article{height:auto;width:100%;}
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