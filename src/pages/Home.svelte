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
          <div style="margin-top:-.2rem;background-size: 2rem;
          background-position: bottom right;border:0.3rem solid white;">
          <p style="">
              <b transition:fade  style="font-weight:900!important;" >POINTBLANK LLC</b> is a Rapid Prototyping, Consulting, and App Development public benefit corporation out of Portland Oregon.
              <br> <br></p> </div>
          <div class="button-row">
          <a href="https://www.prnewswire.com/news-releases/spacex-to-launch-doge-1-to-the-moon-301287016.html"><button>DOGE-1</button></a>
          <a href="https://xiprotocol.io/"><button>XI PROTOCOL</button></a>
          <a href="https://noclip.org/"><button>NOCLIP</button></a>
          <a href="https://revest.finance/"><button>REVEST</button></a>
          <a href="https://rena.finance"><button>RENA</button></a>
          <a href="https://www.olympusdao.finance/"><button>OLYMPUS</button></a>
          <a href="https://www.guranft.com/"><button>GURA NFT</button></a>
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
    padding:0.5rem 0rem;display:flex;flex-flow:row;max-width:100%;
}
article > div > p{
    text-align: left;
    padding:0.3rem 0.5rem;background:white;
    color:rgb(0, 0, 0);margin:unset;
}
.row{display:flex;flex-flow:row;}
.column{display:flex;flex-flow:column;}
.button-row{
    display: flex;
    flex-flow: wrap;
    justify-content: flex-end;
height: fit-content;margin-right: -0.3rem;
margin-top: -0.2rem;
}
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