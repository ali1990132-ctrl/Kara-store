<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1,user-scalable=no">
<meta name="theme-color" content="#060810">
<title>كارة ستور | Kara Store - فاطمة 3</title>
<style>
:root{--bg:#060810;--card:#101522;--muted:#9aa6ba;--pink:#ff2d88;--purple:#9147ff;--green:#16c784;--gold:#ffb020;--cyan:#06b6d4}
*{box-sizing:border-box;margin:0;padding:0;font-family:system-ui,-apple-system,"Segoe UI",Arial,sans-serif}
html{scroll-behavior:smooth}
body{background:radial-gradient(circle at top,#21133d,#080a12 42%,#05060b);color:#fff;max-width:520px;margin:auto;min-height:100vh;padding-bottom:90px;overflow-x:hidden}
a{text-decoration:none;color:inherit;cursor:pointer}
button{font-family:inherit;cursor:pointer}

.header{position:sticky;top:0;z-index:1000;height:68px;padding:8px 14px;display:flex;align-items:center;justify-content:space-between;background:#060810e8;backdrop-filter:blur(20px);border-bottom:1px solid #ffffff12}
.brand h1{font-size:16px;font-weight:1000}
.brand p{font-size:9px;color:var(--muted)}

.hero{position:relative;min-height:650px;display:flex;align-items:center;justify-content:center;text-align:center;overflow:hidden}
.video-bg{position:absolute;inset:0;background:#000}
.video-bg iframe{position:absolute;top:50%;left:50%;width:100vw;height:56.25vw;min-width:177.77vh;min-height:100%;transform:translate(-50%,-50%);border:0;pointer-events:none}
.video-overlay{position:absolute;inset:0;background:linear-gradient(180deg,#05060b18,#05060b35 45%,#05060b80)}

.hero-content{position:relative;z-index:5;width:100%;padding:30px 15px}
.hero h2{font-size:31px;line-height:1.25;font-weight:1000;margin-bottom:12px;text-shadow:0 3px 12px #000}
.hero h2 span{background:linear-gradient(90deg,#fff,#ff62a7,#a970ff);-webkit-background-clip:text;color:transparent}

.hero-sub{font-size:12px;line-height:1.9;max-width:410px;margin:0 auto 20px;padding:8px 12px;border-radius:13px;background:#0005;backdrop-filter:blur(4px)}
.trial-big{margin:18px auto;padding:15px;max-width:390px;border-radius:18px;background:#0c0a0f99;border:1px solid #ffb02088}
.trial-big strong{display:block;font-size:20px;color:#ffd166}
.trial-big span{font-size:10px}

.hero-buttons{display:flex;gap:9px;justify-content:center;flex-wrap:wrap}
.hero-btn{padding:12px 17px;border-radius:14px;font-size:11px;font-weight:1000;display:inline-block}
.whatsapp{background:linear-gradient(135deg,#20d879,#0ca85a)}
.secondary{background:#0007;border:1px solid #fff3}
.sound-btn{position:absolute;z-index:20;bottom:18px;right:15px;border:1px solid #fff4;background:#0009;color:#fff;padding:11px 15px;border-radius:15px;font-size:11px;font-weight:1000}

.search-wrap{padding:12px 15px 5px}
.search-box{width:100%;padding:14px 17px;border-radius:16px;border:1px solid #ffffff1a;background:#101522;color:#fff;outline:none;font-size:12px}

.filter-wrap{display:flex;gap:7px;overflow-x:auto;padding:10px 15px 5px;scrollbar-width:none}
.filter-btn{flex:0 0 auto;border:1px solid #ffffff14;background:#101522;color:#aab5c7;border-radius:12px;padding:8px 12px;font-size:9px;font-weight:900}
.filter-btn.active{background:linear-gradient(135deg,#9147ff,#ff2d88);color:#fff}

.section{padding:18px 15px 8px}
.section-head,.offer-head{display:flex;align-items:center;justify-content:space-between;margin-bottom:12px}
.section-title,.offer-head h2{font-size:19px;font-weight:1000}
.section-note,.offer-head span{font-size:9px;color:var(--muted)}

.features{display:flex;gap:10px;overflow-x:auto;padding:5px 15px 20px}
.feature{min-width:125px;height:105px;border-radius:18px;padding:14px;display:flex;flex-direction:column;justify-content:space-between;background:linear-gradient(145deg,#171d2d,#0d111c);border:1px solid #ffffff12}
.feature-icon{font-size:30px}
.feature strong{font-size:11px}

.offer-section{padding:18px 0 20px;background:linear-gradient(180deg,#ff2d881f,transparent)}
.offer-head{padding:0 15px}
.scroll,.player-scroll,.ai-grid,.ent-grid,.design-grid{display:flex;gap:12px;overflow-x:auto;padding:4px 15px 12px;scrollbar-width:none}
.offer-card,.big-card{flex:0 0 285px;min-height:185px;border-radius:22px;padding:17px;position:relative;overflow:hidden;background:linear-gradient(135deg,#24104c,#15101f);border:1px solid #ffffff20;box-shadow:0 12px 35px #0006}

.offer-icon,.big-icon{width:72px;height:72px;border-radius:20px;display:grid;place-items:center;font-size:38px;background:#ffffff12;border:1px solid #ffffff18;margin-bottom:10px}
.offer-card h3,.big-card h3{font-size:17px;font-weight:1000}
.offer-card p,.big-card p{font-size:10px;color:#cbd5e1;margin-top:4px;line-height:1.7}

.offer-bottom{display:flex;align-items:center;justify-content:space-between;margin-top:12px}
.offer-price{font-size:19px;font-weight:1000;color:#ffd166}

.order-small{display:inline-flex;align-items:center;justify-content:center;color:#fff;background:linear-gradient(135deg,#10b981,#059669);padding:9px 12px;border-radius:10px;font-size:10px;font-weight:1000;border:0;white-space:nowrap}

.iptv-section{background:linear-gradient(180deg,#9147ff1f,transparent)}
.iptv-grid{display:flex;flex-direction:column;gap:14px}
.iptv-card{padding:16px;border-radius:23px;background:linear-gradient(135deg,#1c1430fa,#0a0d17fa);border:1px solid #9147ff66;box-shadow:0 15px 40px #0006}
.iptv-card.best{border-color:#ff2d8866}
.iptv-card.tiger{border-color:#f59e0b66}
.iptv-card.tod{border-color:#06b6d466}
.iptv-card.dream{border-color:#a855f766}

.iptv-main{display:flex;align-items:center;gap:16px}
.iptv-icon{flex:0 0 105px;width:105px;height:105px;border-radius:25px;display:grid;place-items:center;font-size:52px;background:linear-gradient(135deg,#9147ff,#ff2d88)}
.iptv-info{flex:1}
.iptv-card h3{font-size:23px}
.description{font-size:10px;color:var(--muted);line-height:1.7;margin-top:6px}

.price-list{display:grid;grid-template-columns:repeat(2,1fr);gap:8px;margin-top:15px}
.price-box{min-height:53px;padding:7px 8px;border-radius:13px;background:#ffffff08;border:1px solid #ffffff10;display:flex;align-items:center;justify-content:space-between;gap:6px}
.price-info{display:flex;flex-direction:column;gap:2px}
.price-duration{font-size:9px;color:#aab5c7}
.iptv-price{font-size:14px;font-weight:1000;color:#6ee7b7}

.players{background:linear-gradient(180deg,#06b6d41a,transparent)}
.player-card,.ai-card,.ent-card,.design-card{flex:0 0 190px;padding:15px;border-radius:20px;background:linear-gradient(145deg,#101c27,#0c1018);border:1px solid #ffffff12}
.player-icon,.ai-icon,.ent-icon,.design-icon{width:82px;height:82px;margin-bottom:10px;border-radius:20px;display:grid;place-items:center;font-size:40px;background:#ffffff0b}

.player-card h3,.ai-card h3,.ent-card h3,.design-card h3{font-size:15px}
.player-card p,.ai-card p,.ent-card p,.design-card p{font-size:9px;color:var(--muted);margin:4px 0 10px}
.player-price{font-size:16px;color:#22d3ee;font-weight:1000}

.footer{margin:20px 15px;padding:22px;text-align:center;border-radius:22px;background:#0e131f;border:1px solid #ffffff12}
.footer h2{font-size:19px}
.footer p{font-size:10px;color:var(--muted);line-height:1.8;margin-top:7px}
.footer strong{display:block;margin-top:10px;font-size:12px;color:#c084fc}

.bottom{position:fixed;bottom:0;left:50%;transform:translateX(-50%);width:100%;max-width:520px;z-index:1200;display:flex;justify-content:space-around;padding:10px 0 14px;background:#0c101af2;backdrop-filter:blur(20px);border-top:1px solid #ffffff12}
.bottom a{color:#9aa6ba;display:flex;flex-direction:column;align-items:center;gap:4px;font-size:9px;font-weight:800}
.bottom-icon{font-size:19px}
.bottom .active{color:#c084fc}

.float{position:fixed;z-index:1500;width:55px;height:55px;border-radius:50%;display:grid;place-items:center;font-size:25px;box-shadow:0 8px 30px #0007;border:2px solid #fff2}
.float-wa{right:12px;bottom:100px;background:#12c76f}

.cart-fab{position:fixed;right:78px;bottom:104px;z-index:1600;width:55px;height:55px;border-radius:50%;border:2px solid #fff2;background:linear-gradient(135deg,#9147ff,#ff2d88);color:#fff;font-size:23px}
.cart-count{position:absolute;top:-5px;right:-5px;min-width:21px;height:21px;border-radius:20px;background:#ef4444;font-size:10px;font-weight:1000;display:grid;place-items:center}

.cart-overlay{position:fixed;inset:0;background:#0009;z-index:3000;display:none;align-items:flex-end;justify-content:center}
.cart-overlay.show{display:flex}
.cart-modal{width:100%;max-width:520px;max-height:88vh;overflow:auto;background:linear-gradient(180deg,#141a28,#080b12);border:1px solid #ffffff18;border-radius:26px 26px 0 0;padding:18px 15px 25px}
.cart-head{display:flex;align-items:center;justify-content:space-between;margin-bottom:14px}
.cart-head h2{font-size:20px}
.close-cart{border:0;background:#ffffff12;color:#fff;border-radius:10px;width:36px;height:36px}

.cart-empty{text-align:center;padding:35px 10px;color:#9aa6ba;font-size:12px}
.cart-list{display:flex;flex-direction:column;gap:9px}
.cart-item{padding:11px;border-radius:15px;background:#ffffff08;border:1px solid #ffffff10}
.cart-item-top,.cart-item-bottom{display:flex;justify-content:space-between;gap:10px}
.cart-item-bottom{align-items:center;margin-top:9px}
.cart-item-name{font-size:12px;font-weight:1000}
.cart-item-price{font-size:11px;color:#6ee7b7;font-weight:900}
.qty{display:flex;align-items:center;gap:7px}
.qty button{width:27px;height:27px;border:0;border-radius:8px;background:#ffffff12;color:#fff}
.remove-item{border:0;background:#ef444422;color:#fca5a5;border-radius:8px;padding:6px 8px;font-size:9px}

@media(max-width:420px){
.iptv-icon{flex-basis:82px;width:82px;height:82px}
.iptv-card h3{font-size:20px}
.price-list{gap:6px}
.iptv-price{font-size:13px}
}

@media(max-width:360px){
.hero{min-height:610px}
.hero h2{font-size:27px}
.big-card{flex-basis:230px}
.iptv-icon{flex-basis:72px;width:72px;height:72px}
.price-list{grid-template-columns:1fr}
}

.iptv-card-image{
display:block;
width:100%;
height:auto;
aspect-ratio:1536/691;
object-fit:cover;
border-radius:18px;
margin-bottom:14px;
border:1px solid #ffffff18;
box-shadow:0 10px 28px #0005
}
</style>
