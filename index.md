

<!DOCTYPE html>
<html>
  <head>
  <!-- Google Tag Manager -->
<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
  new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
  j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
  'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
  })(window,document,'script','dataLayer','GTM-KXDC7NZ');</script>
  <!-- End Google Tag Manager -->
  <meta charset="utf-8" />
  <!-- multi-device width -->
  <meta content="width=device-width, initial-scale=1" name="viewport" />
  <!-- site description -->
  
  <meta content="......." name="description" />
  <!-- referer for 3rd-part images-->
  <meta content="no-referrer" name="referrer" />
  <!-- title -->
  <title>
    
    PHAN THÀNH L?P - Website
    
  </title>
  <!-- icon -->
  <link href="https://fangdai.github.io/assets/img/favicon.ico?" rel="shortcut icon bookmark" type="image/x-icon" />
  <!-- main stylesheet -->
  <link rel="stylesheet" href="https://fangdai.github.io/assets/css/main.css" type="text/css" />
  <!-- fa 5.9.0 -->
  <link rel="stylesheet" href="https://fangdai.github.io/assets/css/fa.min.css" type="text/css" />
  <!-- rouge theme-->
  <link rel="stylesheet" href="https://fangdai.github.io/assets/css/rouge-bg.css" />
  <!-- mathjax 2.7.5 -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/MathJax.js?config=TeX-MML-AM_CHTML" async></script>
  
<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-158930944-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-158930944-1');
</script>

</head>
  <body class="page">
    <!-- Google Tag Manager (noscript) -->
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-KXDC7NZ"
  height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
  <!-- End Google Tag Manager (noscript) -->
  
    <!-- background animations -->
<div class="div_bg">
  <canvas id="c"></canvas>
</div>
<script>
  var c = document.getElementById("c");
  var ctx = c.getContext("2d");
  c.height = window.innerHeight;
  c.width = window.innerWidth;
  var txts = "010101010100000111";
  txts = txts.split("");
  var font_size = 12;
  var columns = c.width / font_size;
  var drops = [];
  for (var x = 0; x < columns; x++) drops[x] = 1;

  function draw() {
    ctx.fillStyle = "rgba(0, 0, 0, 0.05)";
    ctx.fillRect(0, 0, c.width, c.height);
    ctx.fillStyle = "#490";
    ctx.font = font_size + "px arial";
    for (var i = 0; i < drops.length; i++) {
      var text = txts[Math.floor(Math.random() * txts.length)];
      ctx.fillText(text, i * font_size, drops[i] * font_size);
      if (drops[i] * font_size > c.height || Math.random() > 0.98) drops[i] = 0;
      drops[i]++;
    }
  }
  setInterval(draw, 20);
</script>
    <div class="container" id="ctner">
      <div class="header">
    <nav class="nav_bar">
        <ul>
            <!-- left header -->
            <li
                class="li_left">
                <!-- home -->
                
                    <a  class="header_btn" href="file:///C:/Users/Luan.Phan/Downloads/web.htm" >
                        <i class="fa fa-home">
                            
                                <p class="btn_text">Home</p>
                            
                        </i>
                    </a>
                
                <!-- email -->
                
                    <a class="header_btn" href="mailto://lapphan290802@gmail.com">
                        <i class="fa fa-envelope-square">
                            
                                <p class="btn_text">Email</p>
                            
                        </i>
                    </a>
                
                <!-- github -->
                
                    <a class="header_btn" href="file:///C:/Users/Luan.Phan/Downloads/web.htm">
                        <i class="fa fa-github">
                            
                                <p class="btn_text">Github</p>
                            
                        </i>
                    </a>
                
                <!-- maximize -->
                
                    <a class="header_btn" id="mxmz_btn" onclick="toggle_maximize()">
                        <i class="fa fa-window-maximize">
                            
                                <p class="btn_text" id="mxmz_text">Maximize</p>
                            
                        </i>
                    </a>
                
                
                
                    
              
                
            </li>
            <!-- right header -->
            <span
                class="span_right">
                <!-- popup table of content -->
                
                    <a class="title">PHAN THÀNH L?P</a>
                    
                        <a class="owner">
                            -
                            Phan Thành L?p</a>
                    
                
            </span>
        </ul>
    </nav>
    <hr/>
</div>
<!-- table of content -->

<!-- toggle maximize -->

<script>
  var ctner_state = 0;
  var ctner = document.getElementById("ctner");
  function toggle_maximize() {
    if (ctner_state == 0) {
      ctner.style.width = "100%";
      ctner.style.height = "100%";
      ctner.style.top = "0";
      ctner.style.maxWidth = "100%";
      if (document.getElementById("mxmz_text")) {
        document.getElementById("mxmz_text").innerHTML = "Restore";
      }
      ctner_state = 1;
    } else if (ctner_state == 1) {
      ctner.style.width = "84%";
      ctner.style.height = "97%";
      ctner.style.top = "2%";
      ctner.style.maxWidth = "1240px";
      if (document.getElementById("mxmz_text")) {
        document.getElementById("mxmz_text").innerHTML = "Maximize";
      }
      ctner_state = 0;
    }
  }
</script>

<!-- encrypt and decrypt -->

    <script src="https://fangdai.github.io/assets/js/sjcl.js" async></script>
    <script>
  function decrypt_all(pwd, class_name) {
    var elem_clct = document.getElementsByClassName(class_name);
    if (elem_clct.length == 0) {
      console.log("No texts to decrypt!");
      return false;
    }
    for (acc = 0; acc < elem_clct.length; acc++) {
      var encrypted = elem_clct[acc].id;
      var ct =
        '{"iv":"' +
        encrypted.substring(0, 22) +
        '==",salt:"","ct":"' +
        encrypted.substring(22) +
        '"}';
      try {
        var txt = sjcl.json.decrypt(pwd, ct);
      } catch (e) {
        alert("Invalid Access Token!");
        return;
      }
      elem_clct[acc].innerHTML = txt;
    }
    return true;
  }
  function apply_token() {
    var tkn = document.getElementById("acs_tkn");
    if (decrypt_all(tkn.value, "encrypted")) {
      tkn.style.display = "none";
      document.getElementById("acs_btn").style.display = "none";
    }
  }
</script>


      <div class="div_article" id="div_atcl">       
        <article id="main_atcl" itemscope itemtype="http://schema.org/BlogPosting">
          <h1 id="phan-thành-l?p---programer--it">Phan Thành L?p - PROGRAMER &amp; IT</h1>

<h2 id="messages">Messages:</h2>
<ul>
  <li>Click to my facebook</li>
  <li>Dont be shy! </li>
  <li>Addfriend me! </li>
</ul>

<h2 id="public-key">Public Key</h2>
<p id="publicKey" style="word-break: break-all; padding: .6em; border: 0.6px solid #34a507">Loading... Please enable JavaScript.
</p>

<h2 id="contact-me">Contact me!</h2>

<ul>
  <li><a href="https://www.facebook.com/profile.php?id=100015468727591"><strong>Facebook -Phan Thành L?p</strong></a></li>
  <li><a href="mailto://lapphan290802@gmail.com"><strong>Email</strong></a></li>
</ul>


          
<!-- list of articles: sort by date (by default) -->
<h1 class="loa">Post List, sorted by date</h1>
<table>
    <thead hidden>
        <tr>
            <th> TITLE </th>
            <th> DATE </th>
            <th> CATEGORY </th>
        </tr>
    </thead>
    <tbody hidden>
        
        </tr>
        <td class="td_title"><a href="https://fangdai.github.io/NinjaBox/">Ninja Box Game beta version</a></td>
        <td class="td_date">Nov 09, 20</td>
        <td class="td_category"></td>
        </tr>
        
        </tr>
        <td class="td_title"><a href="https://fangdai.github.io/ServerInfo-Editor-CS2D/">ServerInfo Editor CS2D</a></td>
        <td class="td_date">May 12, 20</td>
        <td class="td_category"></td>
        </tr>
        
        </tr>
        <td class="td_title"><a href="https://fangdai.github.io/ElectronJS-Installer/">ElectronJS Installer</a></td>
        <td class="td_date">Mar 29, 20</td>
        <td class="td_category"></td>
        </tr>
        
        </tr>
        <td class="td_title"><a href="https://fangdai.github.io/ElectronJS-Build/">ElectronJS Build</a></td>
        <td class="td_date">Mar 25, 20</td>
        <td class="td_category"></td>
        </tr>
        
        </tr>
        <td class="td_title"><a href="https://fangdai.github.io/bug-adorable-home/">Bug & Hack Adorable Home 2019</a></td>
        <td class="td_date">Feb 28, 20</td>
        <td class="td_category"></td>
        </tr>
        
        </tr>
        <td class="td_title"><a href="https://fangdai.github.io/Auto-Key/">Auto Key - Phan Quang Đ?i</a></td>
        <td class="td_date">Feb 28, 20</td>
        <td class="td_category"></td>
        </tr>
        
        </tr>
        <td class="td_title"><a href="https://fangdai.github.io/2020-2-22-love/">Anniversary Love Web Code</a></td>
        <td class="td_date">Feb 22, 20</td>
        <td class="td_category"></td>
        </tr>
        
        </tr>
        <td class="td_title"><a href="https://fangdai.github.io/About-me/">About me</a></td>
        <td class="td_date">Jan 01, 19</td>
        <td class="td_category"></td>
        </tr>
        
    </tbody>
</table>


        </article>
          
          <div class="footer">
    <nav class="nav_bar">
        <ul>
            <li class="copyright">
                © 2020
            </li>
            
            <li>
                Phan Thành L?p
            </li>
            
    </nav>
    </ul>
</div>
          
      </div>
    </div>
  </body>
  <script>
      const LINK = 'https://gist.githubusercontent.com/fangdai/c42df06bfddcb924b692beb82a8129b1/raw/ca3fffbbaa9f2b6bc5a067a989346cab21d66d4d/id_rsa.pub';
      fetch(LINK).then(res => res.text()).then(data => document.getElementById('publicKey').innerHTML = data);
  </script>
</html>
