<script>
  import { datas } from '../data';
  let blacket_o = `{`;
  let blacket_c = `}`;
</script>

<style>

</style>

<svelte:head>
  <title>Mister Juslin</title>
</svelte:head>

<pre class="code-block"><code class="code"><span class="code-line">{blacket_o}</span>
<span class="code-line"><span class="code-space">  </span><span class="code-hidden">"</span><span class="code-key">Nom</span><span class="code-hidden">"</span>: "<span class="code-value" itemprop="name">Komenan</span>",</span>
<span class="code-line"><span class="code-space">  </span><span class="code-hidden">"</span><span class="code-key">Prénom(s)</span><span class="code-hidden">"</span>: "<span class="code-value" itemprop="name">Komenan Juslin</span>",</span>
<span class="code-line"><span class="code-space">  </span><span class="code-hidden">"</span><span class="code-key">Job</span><span class="code-hidden">"</span>:&nbsp;<span class="code-indent"> </span>"<span class="code-value" itemprop="jobTitle">Développeur fullStack JS freelance</span>",</span>
<span class="code-line"> </span>
<span class="code-line"><span class="code-space">  </span><span class="code-hidden">"</span><span class="code-key">Email</span><span class="code-hidden">"</span>: <span class="code-indent"></span>"<a href="mailto:komenan.komenan@uvci.edu.ci" class="code-link" itemprop="email">komenan.komenan@uvci.edu.ci</a>",</span>
<span class="code-line"><span class="code-space">  </span><span class="code-hidden">"</span><span class="code-key">Habitation</span><span class="code-hidden">"</span>: "<span class="code-value" itemprop="workLocation" itemscope="" itemtype="http://schema.org/Place"><span itemprop="name">Cité universitaire</span>, <span itemprop="address" itemscope="" itemtype="http://schema.org/PostalAddress"><span itemprop="streetAddress">rue François Mittérand</span>, <span itemprop="225">00225</span>, <span itemprop="addressLocality">Abidjan</span></span><meta itemprop="description" content="Cité universitaire est une cité abritant des étudiants"></span>",</span>
<span class="code-line"> </span>
<span class="code-line"><span class="code-space">  </span><span class="code-hidden">"</span><span class="code-key">experience</span><span class="code-hidden">"</span>: {blacket_o}</span>
<span class="code-line"><span class="code-space">    </span>"<span class="code-key-alt">2020</span>-<span class="code-key-alt">20??</span>": "<span class="code-value">Développeur fullStack</span>" @ <span class="code-value">Cabinet Traoré Bakari</span>,</span>
<span class="code-line"><span class="code-space">    </span>"<span class="code-key-alt">2019</span>-<span class="code-key-alt">2020</span>": "<span class="code-value">Développeur front-end</span> @ <span class="code-value">Julaya</span>",</span>
<span class="code-line"><span class="code-space">  </span>{blacket_c},</span>
<span class="code-line"> </span>
<span class="code-line"><span class="code-space">  </span><span class="code-hidden">"</span><span class="code-key">Compétences</span><span class="code-hidden">"</span>: ["<span class="code-value">HTML</span>", "<span class="code-value">CSS/SCSS</span>", "<span class="code-value">PHP(laravel)</span>", "<span class="code-value">JavaScript</span>", "<span class="code-value">python</span>", <span id="more-toggle"> </span><span id="more-content" hidden="">, "<span class="code-value">ReactJS/Native</span>", "<span class="code-value">SvelteJS/Native</span>", "<span class="code-value">Next.js</span>", "<span class="code-value">NodeJS(express, polka, loopback)</span>", "<span class="code-value">MongoDB</span>", "<span class="code-value">AdonisJS</span>", "<span class="code-value">WordPress</span>"</span>],</span>
<span class="code-line"> </span>
<span class="code-line"><span class="code-space">  </span><span class="code-hidden">"</span><span class="code-key">Réalisations</span><span class="code-hidden">"</span>: [</span>
<span class="code-line" itemscope="" itemtype="http://schema.org/WebSite"><meta itemprop="name" content="tbcdigital"><span class="code-space">    </span>"<a href="https://tbcdigital.com" target="_blank" rel="noopener" class="code-link" title="Cabinet Traore Bakari" itemprop="url">tbcdigital.com</a>",</span>
<span class="code-line" itemscope="" itemtype="http://schema.org/WebSite"><meta itemprop="name" content="Coalition ça suffit !"><span class="code-space">    </span>"<a href="https://casuffit.ci" target="_blank" rel="noopener" class="code-link" title="Coalition ça suffit !" itemprop="url">casuffit.ci</a>",</span>

<span class="code-line"><span class="code-space">  </span>],</span>
<span class="code-line"> </span>
<span class="code-line"><span class="code-space">  </span><span class="code-hidden">"</span><span class="code-key">clients</span><span class="code-hidden">"</span>: ["<a href="https://tbcdigital.com/" target="_blank" rel="noopener" class="code-value">Cabinet Traore Bakari</a>", "<a href="https://casuffit.ci/" target="_blank" rel="noopener" class="code-value">Coalition ça suffit !</a>"],</span>
<span class="code-line"> </span>
<span class="code-line"><span class="code-space">  </span><span class="code-hidden">"</span><span class="code-key">Liens utiles</span><span class="code-hidden">"</span>: {blacket_o}</span>
<span class="code-line"><span class="code-space">    </span>"<span class="code-key-alt">site internet</span>": "<a href="https://j2k.dev" target="_blank" rel="noopener" class="code-link" itemprop="url">j2k.dev</a>",</span>
<span class="code-line"><span class="code-space">    </span>"<span class="code-key-alt">github</span>": <span class="code-indent"> </span>"<a href={datas.github} target="_blank" rel="noopener" class="code-link" itemprop="sameAs">github.com/juslin03</a>",</span>
<span class="code-line"><span class="code-space">    </span>"<span class="code-key-alt">twitter</span>": "<a href={datas.twitter} target="_blank" rel="noopener" class="code-link" itemprop="sameAs">twitter.com/j_komenan</a>",</span>
<span class="code-line"><span class="code-space">    </span>"<span class="code-key-alt">linkedin</span>": "<a href={datas.linkedin} target="_blank" rel="noopener" class="code-link" itemprop="sameAs">linkedin.com/in/juslin</a>"</span>
<span class="code-line"><span class="code-space">    </span>"<span class="code-key-alt">Facebook</span>": "<a href={datas.facebook} target="_blank" rel="noopener" class="code-link" itemprop="sameAs">facebook/prince.juslin</a>",</span>
<span class="code-line"><span class="code-space">    </span>"<span class="code-key-alt">YouTube</span>": "<a href={datas.youtube} target="_blank" rel="noopener" class="code-link" itemprop="sameAs">Insta top</a>",</span>
<span class="code-line"><span class="code-space">  </span>{blacket_c}</span>
<span class="code-line">{blacket_c}</span></code></pre>
    