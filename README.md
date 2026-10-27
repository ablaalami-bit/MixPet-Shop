<!DOCTYPE html>
<html lang="en-GB">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MixPet Shop — Personalised Pet Accessories (EMEA)</title>
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;700;800&display=swap" rel="stylesheet">

<!-- Mixpanel snippet: replace YOUR_PROJECT_TOKEN. If left as-is, events only appear in the on-page debug console. -->
<script>
(function(f,b){if(!b.__SV){var e,g,i,h;window.mixpanel=b;b._i=[];b.init=function(e,f,c){function g(a,d){var b=d.split(".");2==b.length&&(a=a[b[0]],d=b[1]);a[d]=function(){a.push([d].concat(Array.prototype.slice.call(arguments,0)))}}var a=b;"undefined"!==typeof c?a=b[c]=[]:c="mixpanel";a.people=a.people||[];a.toString=function(a){var d="mixpanel";"mixpanel"!==c&&(d+="."+c);a||(d+=" (stub)");return d};a.people.toString=function(){return a.toString(1)+".people (stub)"};i="disable time_event track track_pageview track_links track_forms track_with_groups add_group set_group remove_group register register_once alias unregister identify name_tag set_config reset opt_in_tracking opt_out_tracking has_opted_in_tracking has_opted_out_tracking clear_opt_in_out_tracking start_batch_senders people.set people.set_once people.unset people.increment people.append people.union people.track_charge people.clear_charges people.delete_user people.remove".split(" ");for(h=0;h<i.length;h++)g(a,i[h]);var j="set_config".split(" ");a._i.push([e,f,c])};b.__SV=1.2;e=f.createElement("script");e.type="text/javascript";e.async=!0;e.src="undefined"!==typeof MIXPANEL_CUSTOM_LIB_URL?MIXPANEL_CUSTOM_LIB_URL:"file:"===f.location.protocol&&"//cdn.mxpnl.com/libs/mixpanel-2-latest.min.js".match(/^\/\//)?"https://cdn.mxpnl.com/libs/mixpanel-2-latest.min.js":"//cdn.mxpnl.com/libs/mixpanel-2-latest.min.js";g=f.getElementsByTagName("script")[0];g.parentNode.insertBefore(e,g)}})(document,window.mixpanel||[]);
</script>

<style>
:root{
  --primary:#E5484D; --primary-hover:#C93A3F; --secondary:#12A594;
  --dark:#1A1A1A; --gray:#6B7280; --white:#fff; --light-bg:#FAFAF8;
  --border:#E5E7EB; --radius:16px; --shadow:0 6px 24px rgba(0,0,0,.07);
}
*{box-sizing:border-box;margin:0;padding:0;font-family:'Plus Jakarta Sans',sans-serif}
html{scroll-behavior:smooth}
body{background:var(--light-bg);color:var(--dark);line-height:1.6}
button{font-family:inherit}
.hidden{display:none!important}

.top-bar{background:var(--dark);color:var(--white);text-align:center;padding:8px 16px;font-size:.85rem;font-weight:600}
.top-bar span{color:#FFD166}

header{background:var(--white);border-bottom:1px solid var(--border);position:sticky;top:0;z-index:100}
.nav-container{max-width:1200px;margin:0 auto;display:flex;justify-content:space-between;align-items:center;padding:14px 24px;gap:16px;flex-wrap:wrap}
.logo{font-size:1.5rem;font-weight:800;color:var(--primary);text-decoration:none}
.nav-links{display:flex;gap:22px;list-style:none}
.nav-links a{text-decoration:none;color:var(--dark);font-weight:600;font-size:.95rem}
.nav-links a:hover{color:var(--primary)}
.nav-actions{display:flex;align-items:center;gap:12px}
.region-select{border:1px solid var(--border);background:#E8F5E9;color:#2E7D32;padding:6px 10px;border-radius:20px;font-size:.8rem;font-weight:700;cursor:pointer}
.vip-badge{background:#FFD166;color:#5c4300;padding:4px 10px;border-radius:20px;font-size:.75rem;font-weight:800}
.cart-btn{position:relative;background:var(--dark);color:#fff;border:none;border-radius:10px;padding:9px 16px;font-weight:700;cursor:pointer}
.cart-count{background:var(--primary);color:#fff;border-radius:20px;font-size:.72rem;padding:1px 7px;margin-left:6px}

.hero{background:linear-gradient(135deg,#FFF5F5 0%,#E6FFFA 100%);padding:56px 24px;text-align:center}
.hero-container{max-width:800px;margin:0 auto}
.hero h1{font-size:2.8rem;font-weight:800;line-height:1.2;margin-bottom:16px}
.hero p{font-size:1.1rem;color:var(--gray);margin-bottom:24px}
.hero .btn{width:auto;display:inline-block;padding:14px 32px}

.section{max-width:1200px;margin:48px auto;padding:0 24px}
.section h2{font-size:1.8rem;font-weight:800;margin-bottom:6px}
.section .lead{color:var(--gray);margin-bottom:22px}

/* Shop toolbar */
.toolbar{display:flex;flex-wrap:wrap;gap:10px;align-items:center;margin-bottom:22px}
.chip{border:2px solid var(--border);background:#fff;border-radius:20px;padding:7px 14px;font-weight:700;font-size:.85rem;cursor:pointer}
.chip.active,.chip:hover{border-color:var(--secondary);background:#E6FFFA}
.toolbar input,.toolbar select{padding:9px 14px;border:2px solid var(--border);border-radius:10px;font-size:.9rem}
.toolbar input{flex:1;min-width:180px}

.product-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(235px,1fr));gap:22px}
.product{background:#fff;border:1px solid var(--border);border-radius:var(--radius);overflow:hidden;box-shadow:var(--shadow);display:flex;flex-direction:column;transition:transform .15s}
.product:hover{transform:translateY(-3px)}
.p-img{height:150px;display:flex;align-items:center;justify-content:center;font-size:3.6rem;cursor:pointer}
.p-body{padding:16px;display:flex;flex-direction:column;gap:6px;flex:1}
.p-cat{font-size:.72rem;text-transform:uppercase;letter-spacing:.5px;color:var(--gray);font-weight:700}
.p-name{font-weight:700;cursor:pointer}
.p-price{font-weight:800;font-size:1.1rem}
.p-tag{display:inline-block;background:#FFF3CD;color:#7a5a00;border-radius:6px;font-size:.7rem;font-weight:800;padding:2px 8px;width:fit-content}
.p-body .btn{margin-top:auto}

/* Buttons & forms */
.btn{display:inline-block;width:100%;background:var(--primary);color:#fff;border:none;padding:12px 18px;font-size:.95rem;font-weight:700;border-radius:10px;cursor:pointer;transition:background .2s,transform .1s;text-align:center}
.btn:hover{background:var(--primary-hover)}
.btn:active{transform:scale(.98)}
.btn.secondary{background:#fff;color:var(--dark);border:2px solid var(--border)}
.btn.secondary:hover{background:#f3f4f6}
.btn:disabled{opacity:.5;cursor:not-allowed}
.form-group{margin-bottom:14px}
.form-group label{display:block;font-size:.8rem;font-weight:700;margin-bottom:6px;text-transform:uppercase;letter-spacing:.5px}
.form-control{width:100%;padding:11px 14px;border:2px solid var(--border);border-radius:10px;font-size:.95rem}
.form-control:focus{outline:none;border-color:var(--primary)}
.row2{display:grid;grid-template-columns:1fr 1fr;gap:12px}

.main-container{max-width:1200px;margin:48px auto;padding:0 24px;display:grid;grid-template-columns:1fr 1fr;gap:40px}
@media(max-width:850px){.main-container{grid-template-columns:1fr}.hero h1{font-size:2rem}.nav-links{display:none}}
.card{background:#fff;border-radius:var(--radius);padding:30px;box-shadow:var(--shadow);border:1px solid var(--border)}
.card-title{font-size:1.4rem;font-weight:700;margin-bottom:6px}
.card-subtitle{font-size:.9rem;color:var(--gray);margin-bottom:22px}

/* 3D studio */
.preview-box{background:radial-gradient(circle,#f0f0f0 0%,#e0e0e0 100%);height:240px;border-radius:12px;display:flex;flex-direction:column;justify-content:center;align-items:center;position:relative;margin-bottom:18px;perspective:1000px;overflow:hidden}
.pet-tag-3d{width:140px;height:140px;background:linear-gradient(145deg,#ffd700,#b8860B);border-radius:50%;display:flex;flex-direction:column;justify-content:center;align-items:center;color:#333;box-shadow:0 10px 20px rgba(0,0,0,.2),inset 0 2px 5px rgba(255,255,255,.8);transform-style:preserve-3d;transition:transform .1s ease-out;border:4px solid #daa520}
.tag-hole{width:14px;height:14px;background:#d0d0d0;border-radius:50%;position:absolute;top:12px;box-shadow:inset 0 2px 4px rgba(0,0,0,.4)}
.tag-text-name{font-size:1.2rem;font-weight:800;text-transform:uppercase;letter-spacing:1px;text-shadow:1px 1px 0 rgba(255,255,255,.4);margin-top:10px;max-width:120px;text-align:center;overflow:hidden}
.tag-text-phone{font-size:.75rem;font-weight:700;opacity:.8}
.variant-pill{position:absolute;bottom:8px;right:10px;font-size:.7rem;font-weight:700;color:var(--gray);background:#fff;border-radius:10px;padding:2px 8px}
.species-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin-bottom:16px}
.species-option{border:2px solid var(--border);border-radius:10px;padding:12px;text-align:center;cursor:pointer;transition:all .2s}
.species-option:hover,.species-option.active{border-color:var(--secondary);background:#E6FFFA}
.species-option b{font-size:1.5rem;display:block}
.species-option span{font-size:.8rem;font-weight:700}
.recs{margin-top:18px;display:grid;gap:10px}

/* VIP */
#vip{max-width:1200px;margin:0 auto 48px;padding:0 24px}
.vip-card{background:linear-gradient(135deg,#1A1A1A 0%,#333 100%);color:#fff;border-radius:var(--radius);padding:32px;position:relative;overflow:hidden}
.vip-card::after{content:"PAWS CLUB VIP";position:absolute;right:-20px;bottom:-10px;font-size:3rem;font-weight:900;opacity:.05}
.vip-card ul{margin:14px 0 20px 20px}
.vip-price{font-size:1.9rem;font-weight:800;color:#FFD166;margin:8px 0}
.vip-card .btn{max-width:320px;background:#FFD166;color:#1A1A1A}

/* Drawer & modals */
.overlay{position:fixed;inset:0;background:rgba(0,0,0,.45);z-index:200;display:none}
.overlay.open{display:block}
.drawer{position:fixed;top:0;right:0;bottom:0;width:min(440px,100%);background:#fff;z-index:210;transform:translateX(100%);transition:transform .25s;display:flex;flex-direction:column}
.drawer.open{transform:none}
.drawer-head{padding:18px 22px;border-bottom:1px solid var(--border);display:flex;justify-content:space-between;align-items:center;font-weight:800;font-size:1.2rem}
.drawer-body{padding:18px 22px;overflow-y:auto;flex:1}
.drawer-foot{padding:18px 22px;border-top:1px solid var(--border)}
.x{background:none;border:none;font-size:1.6rem;cursor:pointer}
.line{display:grid;grid-template-columns:52px 1fr auto;gap:12px;padding:12px 0;border-bottom:1px solid var(--border);align-items:center}
.line .em{font-size:2rem;text-align:center}
.line small{color:var(--gray);display:block}
.qty{display:inline-flex;align-items:center;gap:8px;margin-top:4px}
.qty button{width:26px;height:26px;border-radius:6px;border:1px solid var(--border);background:#fff;cursor:pointer;font-weight:800}
.link{background:none;border:none;color:var(--primary);cursor:pointer;font-weight:700;font-size:.8rem}
.sum-row{display:flex;justify-content:space-between;font-size:.92rem;margin:4px 0}
.sum-row.total{font-weight:800;font-size:1.15rem;margin-top:8px}
.green{color:#2E7D32}
.promo-row{display:flex;gap:8px;margin:12px 0}
.promo-row input{flex:1}
.promo-row .btn{width:auto}
.ship-bar{background:#E6FFFA;border-radius:10px;padding:10px 12px;font-size:.85rem;font-weight:600;margin-bottom:14px}
.upsell{background:#FFF8E1;border-radius:10px;padding:10px 12px;font-size:.85rem;margin-top:12px}

.modal{position:fixed;top:50%;left:50%;transform:translate(-50%,-50%);background:#fff;border-radius:var(--radius);width:min(560px,94%);max-height:92vh;overflow-y:auto;z-index:220;padding:28px;display:none}
.modal.open{display:block}
.modal h3{font-size:1.4rem;margin-bottom:4px}
.modal .x{position:absolute;top:10px;right:16px}
.big-em{font-size:5rem;text-align:center;padding:20px;border-radius:12px;margin-bottom:14px}
.pay-methods{display:grid;gap:8px;margin-bottom:14px}
.pay-methods label{border:2px solid var(--border);border-radius:10px;padding:10px 12px;display:flex;gap:10px;cursor:pointer;font-weight:600}
.pay-methods input:checked + span{color:var(--primary)}
.toast{position:fixed;bottom:24px;left:50%;transform:translateX(-50%) translateY(80px);background:var(--dark);color:#fff;padding:12px 20px;border-radius:10px;font-weight:600;z-index:300;transition:transform .25s}
.toast.show{transform:translateX(-50%)}

footer{background:var(--dark);color:#bbb;text-align:center;padding:30px 16px;font-size:.85rem}

/* Debug console */
.analytics-console{max-width:1200px;margin:40px auto;padding:0 24px}
.console-box{background:#1E1E1E;color:#4AF626;font-family:monospace;padding:20px;border-radius:12px;height:200px;overflow-y:auto;font-size:.82rem}
.console-header{display:flex;justify-content:space-between;align-items:center;margin-bottom:10px;color:#333;font-size:.9rem;font-weight:700}
</style>
</head>
<body>

<div class="top-bar">Midsummer EMEA Flash Sale! Use code <span>SUMMER26</span> for 20% off + Free Engraving!</div>

<header>
  <div class="nav-container">
    <a href="#" class="logo">🐾 MixPet Shop</a>
    <ul class="nav-links">
      <li><a href="#shop">Shop</a></li>
      <li><a href="#studio">3D Custom Studio</a></li>
      <li><a href="#profile">Pet Profile</a></li>
      <li><a href="#vip">Paws Club VIP</a></li>
    </ul>
    <div class="nav-actions">
      <span id="vipBadge" class="vip-badge hidden">⭐ VIP</span>
      <select id="countrySel" class="region-select" aria-label="Country"></select>
      <button class="cart-btn" id="cartBtn">🛒 Cart<span class="cart-count" id="cartCount">0</span></button>
    </div>
  </div>
</header>

<section class="hero">
  <div class="hero-container">
    <h1>Bespoke Pet Accessories, Tailored for Your Best Friend.</h1>
    <p>Premium laser-engraved collars, harnesses and ceramic feeders across EMEA. Free shipping over <b id="heroThreshold"></b>.</p>
    <a href="#shop" class="btn">Shop the collection</a>
  </div>
</section>

<!-- SHOP -->
<section class="section" id="shop">
  <h2>Shop</h2>
  <p class="lead">Everything personalised, shipped across the EMEA region.</p>
  <div class="toolbar">
    <div id="catChips"></div>
    <input id="searchBox" placeholder="Search products…" aria-label="Search">
    <select id="sortSel">
      <option value="featured">Featured</option>
      <option value="low">Price: low to high</option>
      <option value="high">Price: high to low</option>
    </select>
  </div>
  <div class="product-grid" id="grid"></div>
</section>

<!-- STUDIO + PROFILE -->
<div class="main-container">
  <div class="card" id="studio">
    <div class="card-title">🎨 3D Engraving Studio</div>
    <div class="card-subtitle">Personalise your brass tag with a live preview.</div>
    <div class="preview-box" id="previewBox">
      <div class="pet-tag-3d" id="tag3d">
        <div class="tag-hole"></div>
        <div class="tag-text-name" id="tagName">HERMES</div>
        <div class="tag-text-phone" id="tagPhone">+44 7911 123456</div>
      </div>
      <span class="variant-pill" id="variantPill"></span>
    </div>
    <div class="form-group"><label>Pet Name</label><input class="form-control" id="inName" maxlength="12" value="Hermes"></div>
    <div class="form-group"><label>Emergency Phone Number</label><input class="form-control" id="inPhone" maxlength="20" value="+44 7911 123456"></div>
    <button class="btn" id="addTagBtn">Add Custom Tag to Cart (<span id="tagPrice"></span>)</button>
  </div>

  <div class="card" id="profile">
    <div class="card-title">🐶 Build Your Pet Profile</div>
    <div class="card-subtitle">Complete your profile to unlock custom breed recommendations.</div>
    <label style="font-size:.8rem;font-weight:700;text-transform:uppercase">Select Pet Species</label>
    <div class="species-grid" id="speciesGrid" style="margin-top:6px">
      <div class="species-option active" data-s="dog"><b>🐕</b><span>Dog</span></div>
      <div class="species-option" data-s="cat"><b>🐈</b><span>Cat</span></div>
      <div class="species-option" data-s="small"><b>🐹</b><span>Small Pet</span></div>
    </div>
    <div class="form-group"><label>Pet Name</label><input class="form-control" id="pfName" placeholder="e.g. Hermes"></div>
    <div class="form-group"><label>Breed Size</label>
      <select class="form-control" id="pfSize">
        <option value="S">Small (e.g. French Bulldog, Pug)</option>
        <option value="M">Medium (e.g. Beagle, Cocker Spaniel)</option>
        <option value="L">Large (e.g. Golden Retriever, German Shepherd)</option>
      </select></div>
    <button class="btn" id="saveProfileBtn">Save Pet Profile</button>
    <div class="recs" id="recs"></div>
  </div>
</div>

<!-- VIP -->
<section id="vip">
  <div class="vip-card">
    <div style="font-size:.8rem;text-transform:uppercase;letter-spacing:1px;opacity:.7">Exclusive Loyalty</div>
    <h2>Paws Club VIP Membership</h2>
    <div class="vip-price">€4.99 / month</div>
    <ul>
      <li>Free Express Shipping across all EMEA</li>
      <li>Free 3D Custom Laser Engraving</li>
      <li>Annual Free Birthday Gift Box</li>
    </ul>
    <button class="btn" id="vipBtn">Subscribe to Paws Club VIP</button>
  </div>
</section>

<section class="analytics-console">
  <div class="console-header"><span style="color:#fff;background:#333;padding:4px 10px;border-radius:6px">Mixpanel Debug Console</span>
    <button class="link" id="clearConsole">Clear</button></div>
  <div class="console-box" id="console">// events will appear here…</div>
</section>

<footer>© 2026 MixPet Shop · EMEA · Demo store — payments are simulated</footer>

<!-- Cart drawer -->
<div class="overlay" id="overlay"></div>
<aside class="drawer" id="drawer" aria-label="Cart">
  <div class="drawer-head"><span>Your Cart</span><button class="x" data-close>×</button></div>
  <div class="drawer-body" id="cartBody"></div>
  <div class="drawer-foot" id="cartFoot"></div>
</aside>

<!-- Product modal -->
<div class="modal" id="prodModal"><button class="x" data-close>×</button><div id="prodModalBody"></div></div>
<!-- Checkout modal -->
<div class="modal" id="checkoutModal"><button class="x" data-close>×</button><div id="checkoutBody"></div></div>
<!-- Newsletter modal -->
<div class="modal" id="newsModal"><button class="x" data-close>×</button>
  <h3>Get 10% Off Your First Order!</h3>
  <p style="color:var(--gray);margin-bottom:16px">Subscribe to our EMEA pet newsletter and receive your exclusive discount code instantly.</p>
  <div class="form-group"><input class="form-control" id="newsEmail" type="email" placeholder="you@email.com"></div>
  <button class="btn" id="newsBtn">Claim 10% Discount Code</button>
</div>
<!-- VIP modal -->
<div class="modal" id="vipModal"><button class="x" data-close>×</button>
  <h3>Join Paws Club VIP</h3>
  <p style="color:var(--gray);margin-bottom:16px">€4.99 / month. Free express shipping and free engraving, applied automatically at checkout.</p>
  <div class="form-group"><label>Email</label><input class="form-control" id="vipEmail" type="email" placeholder="you@email.com"></div>
  <button class="btn" id="vipConfirm">Start membership</button>
</div>

<div class="toast" id="toast"></div>

<script>
/* ================= CONFIG ================= */
const MIXPANEL_TOKEN = 'YOUR_PROJECT_TOKEN';
const ENGRAVING_FEE = 5;             // € per engraved item (free for VIP / SUMMER26)
const PROMOS = { WELCOME10:.10, SUMMER26:.20, BLACKFRIDAY26:.15, REFER_A_PAW:.10 };

const COUNTRIES = {
  'United Kingdom':{region:'UK & Ireland',cur:'GBP',sym:'£',rate:.85,ship:55,shipFee:4.5},
  'Ireland':{region:'UK & Ireland',cur:'EUR',sym:'€',rate:1,ship:55,shipFee:4.5},
  'Germany':{region:'DACH & Benelux',cur:'EUR',sym:'€',rate:1,ship:55,shipFee:4.5,klarna:true},
  'Netherlands':{region:'DACH & Benelux',cur:'EUR',sym:'€',rate:1,ship:55,shipFee:4.5,klarna:true},
  'France':{region:'Central Europe',cur:'EUR',sym:'€',rate:1,ship:55,shipFee:4.5},
  'Poland':{region:'Central Europe',cur:'PLN',sym:'zł',rate:4.3,ship:55,shipFee:4.5},
  'Spain':{region:'Southern Europe',cur:'EUR',sym:'€',rate:1,ship:55,shipFee:4.5},
  'Sweden':{region:'Nordics',cur:'SEK',sym:'kr',rate:11.2,ship:55,shipFee:4.5,klarna:true},
  'UAE':{region:'Gulf Region',cur:'AED',sym:'AED ',rate:4.0,ship:62,shipFee:6,gulf:true},
  'Saudi Arabia':{region:'Gulf Region',cur:'AED',sym:'AED ',rate:4.0,ship:62,shipFee:6,gulf:true}
};

const CATS = ['Collars & Tags','Harnesses & Leashes','Ceramics & Feeders','Smart & GPS','Travel & Lifestyle','Bundles'];
const SIZED = ['S','M','L'];
const PRODUCTS = [
 {id:'brass-tag',name:'Engraved Brass Tag',cat:0,price:15,em:'🏷️',c:'#FFF3CD',eng:true,desc:'Laser-engraved solid brass tag, up to 2 lines.'},
 {id:'steel-tag',name:'Laser Steel Tag',cat:0,price:18,em:'🔖',c:'#E3F2FD',eng:true,desc:'Scratch-resistant stainless steel, deep laser engraving.'},
 {id:'qr-tag',name:'QR Smart Tag',cat:0,price:22,em:'📱',c:'#E8F5E9',desc:'Scan to show your contact details — no battery required.',tag:'Popular'},
 {id:'leather-collar',name:'Custom-Stitched Leather Collar',cat:0,price:45,em:'🦮',c:'#FBE9E7',eng:true,sizes:true,desc:'Full-grain leather with your pet’s name stitched in.'},
 {id:'comfort-harness',name:'Custom-Fit Comfort Harness',cat:1,price:59,em:'🐕',c:'#E6FFFA',sizes:true,desc:'Breed-specific sizing with soft padding and reflective strips.',tag:'Best seller'},
 {id:'night-harness',name:'Reflective Night Harness',cat:1,price:48,em:'🌙',c:'#EDE7F6',sizes:true,desc:'360° reflective strips for evening walks.'},
 {id:'leash',name:'Reflective Leash',cat:1,price:30,em:'➰',c:'#FFF8E1',desc:'1.5 m padded handle, reflective stitching.'},
 {id:'walk-set',name:'Padded Walking Set',cat:1,price:85,em:'🎒',c:'#E0F7FA',sizes:true,desc:'Harness, leash and lead extender in one set.'},
 {id:'ceramic-bowl',name:'Weighted Ceramic Bowl',cat:2,price:32,em:'🥣',c:'#FCE4EC',eng:true,desc:'Non-slip base, custom name lettering.'},
 {id:'wood-stand',name:'Elevated Wooden Stand',cat:2,price:75,em:'🪵',c:'#EFEBE9',desc:'Solid oak stand with two ceramic bowls.'},
 {id:'slow-feeder',name:'Slow Feeder Bowl',cat:2,price:25,em:'🍽️',c:'#F1F8E9',desc:'Maze design to slow down fast eaters.'},
 {id:'gps-collar',name:'GPS Smart Collar',cat:3,price:149,em:'📡',c:'#E3F2FD',sizes:true,desc:'Live location tracking and activity monitoring.',tag:'New'},
 {id:'activity-tag',name:'Activity Monitor Tag',cat:3,price:60,em:'📊',c:'#E8EAF6',desc:'Tracks steps, sleep and play time.'},
 {id:'led-vest',name:'LED Safety Vest',cat:3,price:75,em:'💡',c:'#FFFDE7',sizes:true,desc:'Rechargeable LED strips, visible up to 500 m.'},
 {id:'carrier',name:'Airline-Approved Carrier',cat:4,price:119,em:'🧳',c:'#E0F2F1',desc:'IATA-compliant, ventilated and padded.'},
 {id:'travel-bed',name:'Orthopaedic Travel Bed',cat:4,price:89,em:'🛏️',c:'#F3E5F5',desc:'Memory-foam, folds flat for trips.'},
 {id:'car-seat',name:'Car Seat Protector',cat:4,price:40,em:'🚗',c:'#ECEFF1',desc:'Waterproof, non-slip, fits all cars.'},
 {id:'bottle',name:'Travel Water Bottle',cat:4,price:40,em:'🥤',c:'#E1F5FE',desc:'Leak-proof bottle with fold-out bowl.'},
 {id:'starter-kit',name:'Welcome Starter Kit',cat:5,price:62.9,was:74,em:'🎁',c:'#FFEBEE',eng:true,sizes:true,desc:'Collar + engraved tag + leash, 15% off.',tag:'Save 15%'},
 {id:'custom-tag',name:'3D Studio Custom Tag',cat:0,price:25,em:'✨',c:'#FFF3CD',hidden:true,desc:'Designed in the 3D Engraving Studio.'}
];
const P = Object.fromEntries(PRODUCTS.map(p=>[p.id,p]));

/* ================= STATE ================= */
const $ = s => document.querySelector(s);
const load = (k,d)=>{try{return JSON.parse(localStorage.getItem(k))??d}catch(e){return d}};
const save = (k,v)=>{try{localStorage.setItem(k,JSON.stringify(v))}catch(e){}};
const S = {
  country: load('mp_country','United Kingdom'),
  cart: load('mp_cart',[]),
  promo: load('mp_promo',null),
  vip: load('mp_vip',false),
  profile: load('mp_profile',null),
  variant: load('mp_variant',null) || (Math.random()<.5?'control':'live_3d'),
  species:'dog', cat:-1, q:'', sort:'featured'
};
save('mp_variant',S.variant);

/* ================= ANALYTICS ================= */
const utm = new URLSearchParams(location.search);
const channelMap = {instagram:'Instagram',amazon:'Amazon',refer:'Friend Referral',email:'Email Newsletter'};
const marketing_channel = channelMap[(utm.get('utm_source')||'').toLowerCase()] || (document.referrer? 'Organic Search':'Organic Search');
const platform = /iPhone|iPad/.test(navigator.userAgent)?'iOS App':/Android/.test(navigator.userAgent)?'Android App':'Web';
const supers = ()=>({country:S.country, region:COUNTRIES[S.country].region, platform, marketing_channel,
  account_status:S.vip?'Subscriber (Paws Club VIP)':'Guest / Unregistered', experiment_variant:S.variant});
const HAS_MP = MIXPANEL_TOKEN && MIXPANEL_TOKEN!=='YOUR_PROJECT_TOKEN';
if(HAS_MP) mixpanel.init(MIXPANEL_TOKEN,{track_pageview:true,persistence:'localStorage'});
function track(name,props={}){
  const payload = Object.assign({}, supers(), props);
  if(HAS_MP) { mixpanel.register(supers()); mixpanel.track(name,props); }
  const c = $('#console'); const line=document.createElement('div');
  line.textContent = `[${new Date().toLocaleTimeString()}] ${name} ${JSON.stringify(payload)}`;
  c.appendChild(line); c.scrollTop=c.scrollHeight;
}

/* ================= HELPERS ================= */
const C = ()=>COUNTRIES[S.country];
const money = eur => { const c=C(); const v=eur*c.rate; return c.sym+(c.rate>=4?v.toFixed(c.cur==='AED'?0:0):v.toFixed(2)); };
const toast = m=>{const t=$('#toast');t.textContent=m;t.classList.add('show');clearTimeout(t._t);t._t=setTimeout(()=>t.classList.remove('show'),2200)};
const lineKey = (id,size,eng)=>[id,size||'',eng||''].join('|');
function freeEngraving(){ return S.vip || S.promo==='SUMMER26'; }

/* ================= CART MATH ================= */
function calc(){
  let sub=0, eng=0;
  S.cart.forEach(l=>{ const p=P[l.id]; sub+=p.price*l.qty; if(l.eng && !freeEngraving()) eng+=ENGRAVING_FEE*l.qty; });
  const disc = S.promo? sub*PROMOS[S.promo] : 0;
  const after = sub-disc+eng;
  const c=C();
  const subForShip = sub-disc; // threshold on discounted merchandise value
  const free = S.vip || subForShip>=c.ship;
  const ship = S.cart.length===0?0:(free?0:c.shipFee);
  return {sub,disc,eng,ship,total:after+ship,free,toFree:Math.max(0,c.ship-subForShip)};
}

/* ================= RENDER: SHOP ================= */
function renderChips(){
  $('#catChips').innerHTML = ['All',...CATS].map((n,i)=>`<button class="chip ${S.cat===i-1?'active':''}" data-c="${i-1}">${n}</button>`).join(' ');
}
function renderGrid(){
  let list = PRODUCTS.filter(p=>!p.hidden && (S.cat<0||p.cat===S.cat) && p.name.toLowerCase().includes(S.q.toLowerCase()));
  if(S.sort==='low') list.sort((a,b)=>a.price-b.price);
  if(S.sort==='high') list.sort((a,b)=>b.price-a.price);
  $('#grid').innerHTML = list.map(p=>`
   <div class="product">
     <div class="p-img" style="background:${p.c}" data-view="${p.id}">${p.em}</div>
     <div class="p-body">
       <span class="p-cat">${CATS[p.cat]}</span>
       <span class="p-name" data-view="${p.id}">${p.name}</span>
       ${p.tag?`<span class="p-tag">${p.tag}</span>`:''}
       <span class="p-price">${money(p.price)} ${p.was?`<s style="color:var(--gray);font-weight:400;font-size:.85rem">${money(p.was)}</s>`:''}</span>
       <button class="btn" data-view="${p.id}">${p.eng||p.sizes?'Customise':'Add to cart'}</button>
     </div>
   </div>`).join('') || '<p>No products match your search.</p>';
}

/* ================= PRODUCT MODAL ================= */
let pm = null;
function openProduct(id){
  const p=P[id]; pm={id,size:S.profile?.size||'M',eng:''};
  track('Product Viewed',{product_id:id,product_name:p.name,category:CATS[p.cat],price_eur:p.price});
  $('#prodModalBody').innerHTML = `
    <div class="big-em" style="background:${p.c}">${p.em}</div>
    <h3>${p.name}</h3>
    <p style="color:var(--gray);margin-bottom:10px">${p.desc}</p>
    <div class="p-price" style="margin-bottom:14px">${money(p.price)}</div>
    ${p.sizes?`<div class="form-group"><label>Size</label><select class="form-control" id="pmSize">${SIZED.map(s=>`<option ${s===pm.size?'selected':''} value="${s}">${{S:'Small',M:'Medium',L:'Large'}[s]}</option>`).join('')}</select></div>`:''}
    ${p.eng?`<div class="form-group"><label>Engraving text <small style="text-transform:none">(${freeEngraving()?'free for you':'+ '+money(ENGRAVING_FEE)})</small></label><input class="form-control" id="pmEng" maxlength="24" placeholder="e.g. Hermes · +44 7911 123456"></div>`:''}
    <button class="btn" id="pmAdd">Add to cart</button>`;
  openModal('#prodModal');
  const sz=$('#pmSize'); if(sz) sz.onchange=()=>pm.size=sz.value;
  const en=$('#pmEng'); if(en) en.oninput=()=>pm.eng=en.value.trim();
  $('#pmAdd').onclick=()=>{
    if(p.eng && pm.eng) track('Product Customized',{product_id:id,engraving_length:pm.eng.length});
    addToCart(id,{size:p.sizes?pm.size:'',eng:pm.eng}); closeAll(); openCart();
  };
}

/* ================= CART ================= */
function addToCart(id,{size='',eng='',name=''}={}){
  const k=lineKey(id,size,eng+name), ex=S.cart.find(l=>l.key===k);
  if(ex) ex.qty++; else S.cart.push({key:k,id,qty:1,size,eng:eng||name,name});
  persist();
  const p=P[id];
  track('Item Added to Cart',{product_id:id,product_name:p.name,category:CATS[p.cat],price_eur:p.price,size});
  if(eng) track('Personalization Applied',{product_id:id,engraving_length:eng.length,experiment_variant:S.variant});
  renderCart(); toast(p.name+' added to cart');
}
function persist(){ save('mp_cart',S.cart); save('mp_promo',S.promo); save('mp_vip',S.vip); save('mp_profile',S.profile); save('mp_country',S.country); }
function renderCart(){
  const n=S.cart.reduce((a,l)=>a+l.qty,0); $('#cartCount').textContent=n;
  const body=$('#cartBody'), foot=$('#cartFoot');
  if(!S.cart.length){ body.innerHTML='<p style="color:var(--gray);padding:20px 0">Your cart is empty. 🐾</p>'; foot.innerHTML=''; return; }
  const t=calc(), c=C();
  const hasHarness=S.cart.some(l=>P[l.id].cat===1), hasTag=S.cart.some(l=>l.id.includes('tag'));
  body.innerHTML = `
   <div class="ship-bar">${t.free?'🚚 You’ve got free shipping!':`Add ${money(t.toFree)} more for free shipping (over ${money(c.ship)})`}</div>
   ${S.cart.map((l,i)=>{const p=P[l.id];return `
    <div class="line">
      <div class="em">${p.em}</div>
      <div><b>${l.name||p.name}</b>
        <small>${[l.size&&({S:'Small',M:'Medium',L:'Large'}[l.size]),l.eng&&'“'+l.eng+'”'].filter(Boolean).join(' · ')}</small>
        <div class="qty"><button data-q="${i}" data-d="-1">−</button>${l.qty}<button data-q="${i}" data-d="1">+</button> <button class="link" data-rm="${i}">Remove</button></div>
      </div>
      <b>${money(p.price*l.qty)}</b>
    </div>`}).join('')}
   ${hasHarness&&!hasTag?`<div class="upsell">💡 Add a matching personalised tag for ${money(P['brass-tag'].price)} <button class="link" data-add="brass-tag">Add</button></div>`:''}`;
  foot.innerHTML = `
   <div class="promo-row"><input class="form-control" id="promoIn" placeholder="Promo code" value="${S.promo||''}"><button class="btn secondary" id="promoBtn">Apply</button></div>
   <div class="sum-row"><span>Subtotal</span><span>${money(t.sub)}</span></div>
   ${t.disc?`<div class="sum-row green"><span>Discount (${S.promo})</span><span>−${money(t.disc)}</span></div>`:''}
   ${t.eng?`<div class="sum-row"><span>Engraving</span><span>${money(t.eng)}</span></div>`:''}
   <div class="sum-row"><span>Shipping${S.vip?' (VIP express)':''}</span><span>${t.ship?money(t.ship):'Free'}</span></div>
   <div class="sum-row total"><span>Total</span><span>${money(t.total)}</span></div>
   <button class="btn" id="checkoutBtn" style="margin-top:12px">Checkout</button>`;
}
function applyPromo(code){
  code=(code||'').trim().toUpperCase();
  if(!code){S.promo=null;persist();renderCart();return}
  if(!PROMOS[code]){toast('Sorry, that code isn’t valid');return}
  S.promo=code; persist(); renderCart(); toast(code+' applied');
  track('Summer Pet Discount Code Applied',{code,discount_pct:PROMOS[code]*100});
}

/* ================= CHECKOUT ================= */
function openCheckout(){
  if(!S.cart.length) return;
  const t=calc(), c=C();
  track('Checkout Started',{cart_value_eur:+t.total.toFixed(2),items:S.cart.reduce((a,l)=>a+l.qty,0),promo:S.promo||'none'});
  $('#checkoutBody').innerHTML=`
   <h3>Checkout</h3><p style="color:var(--gray);margin-bottom:14px">Total: <b>${money(t.total)}</b> · shipping to ${S.country}</p>
   <div class="row2"><div class="form-group"><label>First name</label><input class="form-control" id="ckF"></div><div class="form-group"><label>Last name</label><input class="form-control" id="ckL"></div></div>
   <div class="form-group"><label>Email</label><input class="form-control" id="ckE" type="email"></div>
   <div class="form-group"><label>Address</label><input class="form-control" id="ckA"></div>
   <div class="row2"><div class="form-group"><label>City</label><input class="form-control" id="ckC"></div><div class="form-group"><label>Postcode</label><input class="form-control" id="ckP"></div></div>
   <label style="font-size:.8rem;font-weight:700;text-transform:uppercase">Payment</label>
   <div class="pay-methods" style="margin-top:6px">
     <label><input type="radio" name="pay" value="Card" checked><span>💳 Card</span></label>
     ${c.klarna?'<label><input type="radio" name="pay" value="Klarna invoice"><span>🧾 Klarna invoice</span></label>':''}
     <label><input type="radio" name="pay" value="Apple Pay"><span> Apple Pay</span></label>
   </div>
   <p style="font-size:.75rem;color:var(--gray);margin-bottom:12px">Demo store: no real payment is taken.</p>
   <button class="btn" id="placeOrder">Place order · ${money(t.total)}</button>`;
  closeAll(); openModal('#checkoutModal');
  $('#placeOrder').onclick=()=>{
    const req=['#ckF','#ckE','#ckA','#ckC','#ckP'];
    if(req.some(s=>!$(s).value.trim()) || !/\S+@\S+\.\S+/.test($('#ckE').value)){toast('Please complete all fields with a valid email');return}
    const pay=document.querySelector('input[name=pay]:checked').value;
    const id='MP-'+Math.random().toString(36).slice(2,8).toUpperCase();
    const fin=calc();
    track('Order Completed',{order_id:id,revenue_eur:+fin.total.toFixed(2),items:S.cart.reduce((a,l)=>a+l.qty,0),payment_method:pay,promo:S.promo||'none',is_gift_order:false,experiment_variant:S.variant});
    if(HAS_MP){ mixpanel.identify($('#ckE').value.trim()); mixpanel.people.set({$email:$('#ckE').value.trim(),$name:$('#ckF').value+' '+$('#ckL').value,country:S.country}); }
    S.cart=[]; persist(); renderCart();
    $('#checkoutBody').innerHTML=`<div style="text-align:center;padding:20px 0"><div style="font-size:3.5rem">🎉</div><h3>Thank you!</h3>
      <p style="color:var(--gray);margin:8px 0 18px">Order <b>${id}</b> is confirmed. A receipt is on its way to ${$('#ckE').value}.</p>
      <button class="btn" data-close>Keep shopping</button></div>`;
  };
}

/* ================= MODALS ================= */
function openModal(s){ $('#overlay').classList.add('open'); $(s).classList.add('open'); }
function openCart(){ $('#overlay').classList.add('open'); $('#drawer').classList.add('open'); }
function closeAll(){ document.querySelectorAll('.modal,.drawer,.overlay').forEach(e=>e.classList.remove('open')); }

/* ================= 3D STUDIO ================= */
function initStudio(){
  const box=$('#previewBox'), tag=$('#tag3d');
  $('#variantPill').textContent = S.variant==='live_3d'?'Live 3D preview':'Static preview';
  if(S.variant==='live_3d'){
    box.addEventListener('mousemove',e=>{const r=box.getBoundingClientRect();const x=(e.clientX-r.left)/r.width-.5,y=(e.clientY-r.top)/r.height-.5;tag.style.transform=`rotateY(${x*50}deg) rotateX(${-y*50}deg)`});
    box.addEventListener('mouseleave',()=>tag.style.transform='');
  }
  const upd=()=>{$('#tagName').textContent=$('#inName').value||'NAME';$('#tagPhone').textContent=$('#inPhone').value||''};
  $('#inName').oninput=upd; $('#inPhone').oninput=upd; upd();
  $('#addTagBtn').onclick=()=>{
    const n=$('#inName').value.trim(), ph=$('#inPhone').value.trim();
    if(!n){toast('Please enter your pet’s name');return}
    addToCart('custom-tag',{eng:n+' · '+ph,name:'Custom Tag — '+n}); openCart();
  };
}

/* ================= PET PROFILE ================= */
function renderRecs(){
  if(!S.profile){$('#recs').innerHTML='';return}
  const {species,size,name}=S.profile;
  const ids = species==='dog' ? ['comfort-harness','leather-collar','gps-collar'] : species==='cat' ? ['qr-tag','slow-feeder','travel-bed'] : ['slow-feeder','carrier','bottle'];
  $('#recs').innerHTML = `<b>Picked for ${name||'your pet'}:</b>`+ids.map(i=>`<div class="line" style="grid-template-columns:40px 1fr auto"><div class="em">${P[i].em}</div><div><b>${P[i].name}</b><small>${money(P[i].price)}</small></div><button class="link" data-view="${i}">View</button></div>`).join('');
}

/* ================= EVENTS ================= */
document.addEventListener('click',e=>{
  const t=e.target;
  if(t.closest('[data-close]')||t===$('#overlay')) return closeAll();
  const c=t.closest('[data-c]'); if(c){S.cat=+c.dataset.c;renderChips();renderGrid();return}
  const v=t.closest('[data-view]'); if(v){openProduct(v.dataset.view);return}
  const q=t.closest('[data-q]'); if(q){const l=S.cart[+q.dataset.q];l.qty+=+q.dataset.d;if(l.qty<1)S.cart.splice(+q.dataset.q,1);persist();renderCart();return}
  const rm=t.closest('[data-rm]'); if(rm){S.cart.splice(+rm.dataset.rm,1);persist();renderCart();return}
  const ad=t.closest('[data-add]'); if(ad){addToCart(ad.dataset.add,{});return}
  if(t.id==='promoBtn') return applyPromo($('#promoIn').value);
  if(t.id==='checkoutBtn') return openCheckout();
  const sp=t.closest('.species-option'); if(sp){document.querySelectorAll('.species-option').forEach(x=>x.classList.remove('active'));sp.classList.add('active');S.species=sp.dataset.s}
});
$('#cartBtn').onclick=openCart;
$('#searchBox').oninput=e=>{S.q=e.target.value;renderGrid()};
$('#sortSel').onchange=e=>{S.sort=e.target.value;renderGrid()};
$('#clearConsole').onclick=()=>$('#console').innerHTML='';
$('#countrySel').innerHTML=Object.keys(COUNTRIES).map(k=>`<option ${k===S.country?'selected':''}>${k}</option>`).join('');
$('#countrySel').onchange=e=>{S.country=e.target.value;persist();refreshAll();track('Country Changed',{country:S.country})};

$('#saveProfileBtn').onclick=()=>{
  S.profile={species:S.species,size:$('#pfSize').value,name:$('#pfName').value.trim()};
  persist(); renderRecs(); toast('Pet profile saved 🐾');
  track('Pet Profile Created',{species:S.species,breed_size:S.profile.size,pet_profile_completeness:S.profile.name?'Complete Profile':'Incomplete / Guest'});
};
$('#vipBtn').onclick=()=>{ if(S.vip){toast('You’re already a VIP ⭐');return} openModal('#vipModal'); };
$('#vipConfirm').onclick=()=>{
  if(!/\S+@\S+\.\S+/.test($('#vipEmail').value)){toast('Please enter a valid email');return}
  S.vip=true; persist(); closeAll(); refreshAll(); toast('Welcome to Paws Club VIP! ⭐');
  track('VIP Club Subscribed',{plan:'monthly',price_eur:4.99,pet_profile_completeness:S.profile?'Complete Profile':'Incomplete / Guest'});
};
$('#newsBtn').onclick=()=>{
  if(!/\S+@\S+\.\S+/.test($('#newsEmail').value)){toast('Please enter a valid email');return}
  S.promo='WELCOME10'; persist(); closeAll(); renderCart(); toast('WELCOME10 applied to your cart!');
  track('Newsletter Subscribed',{source:'popup'});
};

function refreshAll(){
  $('#vipBadge').classList.toggle('hidden',!S.vip);
  $('#vipBtn').textContent = S.vip?'You’re a VIP ⭐':'Subscribe to Paws Club VIP';
  $('#heroThreshold').textContent = money(C().ship);
  $('#tagPrice').textContent = money(25);
  renderGrid(); renderCart(); renderRecs();
}

/* ================= INIT ================= */
renderChips(); initStudio(); refreshAll();
track('Page Viewed',{path:location.pathname+location.hash});
if(!sessionStorage.getItem('mp_news')){ setTimeout(()=>{ if(!document.querySelector('.modal.open')){openModal('#newsModal');} sessionStorage.setItem('mp_news','1'); },8000); }
</script>
</body>
</html>
