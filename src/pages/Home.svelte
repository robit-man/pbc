<script>
import { onMount } from "svelte";
import { slide, fade } from 'svelte/transition';
import { Router, Link, Route } from "svelte-routing";

</script>

<main>
  <div class="wrapper">
      <header>
          <img transition:slide src="/imgs/pbc(1).svg" alt="">
      </header>
      <article>
          <div style="margin-bottom: 1.7rem;margin-top:-.2rem;max-width: 512px;">
          <p style="clip-path: polygon(100% 0, 100% calc(100% - 1rem), calc(100% - 1rem) 100%, 0 100%, 0 0);">
              <b transition:fade  style="" >POINTBLANK LLC</b> is a Rapid Prototyping, Consulting, and App Development public benefit corporation out of Portland Oregon.
              <br></p> 
            <div class="line" style=""></div>
            </div>
          <div class="button-row">
          <a href="https://www.prnewswire.com/news-releases/spacex-to-launch-doge-1-to-the-moon-301287016.html"><button>DOGE-1</button></a><div class="crosshair" style="margin-right:0.3rem;"></div>
          <a href="https://xiprotocol.io/"><button>XI PROTOCOL</button></a>
          <a href="https://noclip.org/"><button>NOCLIP</button></a>
          <a href="https://revest.finance/"><button>REVEST</button></a><div class="crosshair" style="margin-right:0.3rem;"></div>
          <a href="https://rena.finance"><button>RENA</button></a>
          <a href="https://www.olympusdao.finance/"><button>OLYMPUS</button></a>
          <a href="https://www.guranft.com/"><button>GURA NFT</button></a>        <div class="crosshair" style="margin-right:0.3rem;"></div>

        </div>
    </article>
    
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
.wrapper{max-width:1024px;
    padding:1rem;
    margin: auto;
    overflow-x: hidden;
}
@keyframes slide{
    0%{background-position-x: 0rem;}
    100%{background-position-x: 2rem;}
}
header{
    margin-top:6rem;
    background:black;
    width:auto;
    padding:0rem;
    height:auto;
    display: flex;
    flex-flow: row;
    justify-content: flex-start;
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
header > img{width:100%;height:auto;
    height:inherit;

}
.line{clip-path: polygon(0 0, calc(100% - 1rem) 0%, 100% 1rem, 100% 100%, 1rem 100%, 0 calc(100% - 1rem));animation:slide 1s linear infinite;background-image:url(/imgs/repeatline.svg);background-size:1rem;margin-top:1.3rem;background-color:white;height:4rem;width:100%;}
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
    padding:0.5rem 0rem;display:flex;flex-flow:wrap;max-width:100%;
    margin-top:1rem;
}
article > div > p{line-height: 1.2;
    text-align: left;text-transform:uppercase;
   
    color:rgb(255, 255, 255);margin:unset;
margin-bottom: unset !important;
}
.row{display:flex;flex-flow:row;}
.column{display:flex;flex-flow:column;}
.button-row{
    display: flex;
    flex-flow: wrap;
    justify-content: flex-end;max-width: 512px;
height: fit-content;margin-right: -0.3rem;
margin-top: -0.2rem;
}.crosshair{background-image:url(/imgs/crosshair.svg); width:2.3rem;height:2.3rem;background-size:2.3rem;filter:invert(1);transition:all 0.2s ease;}.crosshair:hover{clip-path: polygon(0 0, calc(100% - 1rem) 0%, 100% 1rem, 100% 100%, 1rem 100%, 0 calc(100% - 1rem));}
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
.button-row > a {margin-right:0.3rem;
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
    header{
    padding:0rem;
    display: flex;
    flex-flow: row;
    justify-content: center;
    clip-path: unset;
    pointer-events: none;
    border-top-right-radius: unset;
    margin-top: 0rem;
    }
}

</style>