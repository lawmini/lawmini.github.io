<!DOCTYPE html>
<html lang="en" dir="ltr" prefix="content: http://purl.org/rss/1.0/modules/content/  dc: http://purl.org/dc/terms/  foaf: http://xmlns.com/foaf/0.1/  og: http://ogp.me/ns#  rdfs: http://www.w3.org/2000/01/rdf-schema#  schema: http://schema.org/  sioc: http://rdfs.org/sioc/ns#  sioct: http://rdfs.org/sioc/types#  skos: http://www.w3.org/2004/02/skos/core#  xsd: http://www.w3.org/2001/XMLSchema# ">
  <head>
    <meta charset="utf-8" /><script type="text/javascript">window.NREUM||(NREUM={}),__nr_require=function(e,t,n){function r(n){if(!t[n]){var o=t[n]={exports:{}};e[n][0].call(o.exports,function(t){var o=e[n][1][t];return r(o||t)},o,o.exports)}return t[n].exports}if("function"==typeof __nr_require)return __nr_require;for(var o=0;o<n.length;o++)r(n[o]);return r}({1:[function(e,t,n){function r(){}function o(e,t,n){return function(){return i(e,[f.now()].concat(u(arguments)),t?null:this,n),t?void 0:this}}var i=e("handle"),a=e(2),u=e(3),c=e("ee").get("tracer"),f=e("loader"),s=NREUM;"undefined"==typeof window.newrelic&&(newrelic=s);var p=["setPageViewName","setCustomAttribute","setErrorHandler","finished","addToTrace","inlineHit","addRelease"],d="api-",l=d+"ixn-";a(p,function(e,t){s[t]=o(d+t,!0,"api")}),s.addPageAction=o(d+"addPageAction",!0),s.setCurrentRouteName=o(d+"routeName",!0),t.exports=newrelic,s.interaction=function(){return(new r).get()};var m=r.prototype={createTracer:function(e,t){var n={},r=this,o="function"==typeof t;return i(l+"tracer",[f.now(),e,n],r),function(){if(c.emit((o?"":"no-")+"fn-start",[f.now(),r,o],n),o)try{return t.apply(this,arguments)}catch(e){throw c.emit("fn-err",[arguments,this,e],n),e}finally{c.emit("fn-end",[f.now()],n)}}}};a("setName,setAttribute,save,ignore,onEnd,getContext,end,get".split(","),function(e,t){m[t]=o(l+t)}),newrelic.noticeError=function(e){"string"==typeof e&&(e=new Error(e)),i("err",[e,f.now()])}},{}],2:[function(e,t,n){function r(e,t){var n=[],r="",i=0;for(r in e)o.call(e,r)&&(n[i]=t(r,e[r]),i+=1);return n}var o=Object.prototype.hasOwnProperty;t.exports=r},{}],3:[function(e,t,n){function r(e,t,n){t||(t=0),"undefined"==typeof n&&(n=e?e.length:0);for(var r=-1,o=n-t||0,i=Array(o<0?0:o);++r<o;)i[r]=e[t+r];return i}t.exports=r},{}],4:[function(e,t,n){t.exports={exists:"undefined"!=typeof window.performance&&window.performance.timing&&"undefined"!=typeof window.performance.timing.navigationStart}},{}],ee:[function(e,t,n){function r(){}function o(e){function t(e){return e&&e instanceof r?e:e?c(e,u,i):i()}function n(n,r,o,i){if(!d.aborted||i){e&&e(n,r,o);for(var a=t(o),u=m(n),c=u.length,f=0;f<c;f++)u[f].apply(a,r);var p=s[y[n]];return p&&p.push([b,n,r,a]),a}}function l(e,t){v[e]=m(e).concat(t)}function m(e){return v[e]||[]}function w(e){return p[e]=p[e]||o(n)}function g(e,t){f(e,function(e,n){t=t||"feature",y[n]=t,t in s||(s[t]=[])})}var v={},y={},b={on:l,emit:n,get:w,listeners:m,context:t,buffer:g,abort:a,aborted:!1};return b}function i(){return new r}function a(){(s.api||s.feature)&&(d.aborted=!0,s=d.backlog={})}var u="nr@context",c=e("gos"),f=e(2),s={},p={},d=t.exports=o();d.backlog=s},{}],gos:[function(e,t,n){function r(e,t,n){if(o.call(e,t))return e[t];var r=n();if(Object.defineProperty&&Object.keys)try{return Object.defineProperty(e,t,{value:r,writable:!0,enumerable:!1}),r}catch(i){}return e[t]=r,r}var o=Object.prototype.hasOwnProperty;t.exports=r},{}],handle:[function(e,t,n){function r(e,t,n,r){o.buffer([e],r),o.emit(e,t,n)}var o=e("ee").get("handle");t.exports=r,r.ee=o},{}],id:[function(e,t,n){function r(e){var t=typeof e;return!e||"object"!==t&&"function"!==t?-1:e===window?0:a(e,i,function(){return o++})}var o=1,i="nr@id",a=e("gos");t.exports=r},{}],loader:[function(e,t,n){function r(){if(!x++){var e=h.info=NREUM.info,t=d.getElementsByTagName("script")[0];if(setTimeout(s.abort,3e4),!(e&&e.licenseKey&&e.applicationID&&t))return s.abort();f(y,function(t,n){e[t]||(e[t]=n)}),c("mark",["onload",a()+h.offset],null,"api");var n=d.createElement("script");n.src="https://"+e.agent,t.parentNode.insertBefore(n,t)}}function o(){"complete"===d.readyState&&i()}function i(){c("mark",["domContent",a()+h.offset],null,"api")}function a(){return E.exists&&performance.now?Math.round(performance.now()):(u=Math.max((new Date).getTime(),u))-h.offset}var u=(new Date).getTime(),c=e("handle"),f=e(2),s=e("ee"),p=window,d=p.document,l="addEventListener",m="attachEvent",w=p.XMLHttpRequest,g=w&&w.prototype;NREUM.o={ST:setTimeout,SI:p.setImmediate,CT:clearTimeout,XHR:w,REQ:p.Request,EV:p.Event,PR:p.Promise,MO:p.MutationObserver};var v=""+location,y={beacon:"bam.nr-data.net",errorBeacon:"bam.nr-data.net",agent:"js-agent.newrelic.com/nr-1071.min.js"},b=w&&g&&g[l]&&!/CriOS/.test(navigator.userAgent),h=t.exports={offset:u,now:a,origin:v,features:{},xhrWrappable:b};e(1),d[l]?(d[l]("DOMContentLoaded",i,!1),p[l]("load",r,!1)):(d[m]("onreadystatechange",o),p[m]("onload",r)),c("mark",["firstbyte",u],null,"api");var x=0,E=e(4)},{}]},{},["loader"]);</script>
<meta name="title" content="SEC.gov | HOME" />
<link rel="shortlink" href="https://www.sec.gov/" />
<link rel="canonical" href="https://www.sec.gov/" />
<meta name="Generator" content="Drupal 8 (https://www.drupal.org)" />
<meta name="MobileOptimized" content="width" />
<meta name="HandheldFriendly" content="true" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<meta name="id" content="2431" />
<meta name="date" content="2017-02-05T05:36:00" />
<link rel="shortcut icon" href="/themes/custom/secgov/favicon.ico" type="image/vnd.microsoft.icon" />
<link rel="canonical" href="/page/homepage" />
<link rel="shortlink" href="/node/2431" />
<link rel="revision" href="/page/homepage" />
<script src="/files/google_tag/google_tag.script.js?p83pvq"></script>

    <meta name="origin" content="Drupal" />
    <meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate">
    <meta http-equiv="Pragma" CONTENT="no-cache">
    <meta http-equiv="Expires" CONTENT="-1">
    <meta name="viewport" content="width=device-width initial-scale=1.0 maximum-scale=3.0" />
    <title>SEC.gov | HOME</title>
    <script>window.env = "production";</script> 
    <link rel="stylesheet" href="/files/css/css_E1q5Z2tc0kI_jKxTdnsCmPRlaUTahU3z74eRGBK6XgU.css?p83pvq" media="all" />
<link rel="stylesheet" href="/files/css/css_BEluPh_zLnuilDM6A-g0YGkSKHPExYD1w0woK5B_Sq8.css?p83pvq" media="all" />

    
<!--[if lte IE 8]>
<script src="/files/js/js_VtafjXmRvoUgAzqzYTA3Wrjkx9wcWhjP0G4ZnnqRamA.js"></script>
<![endif]-->
<script src="/files/js/js_M8bMkMWYaa6GjkCVIa45Had-OgBsWiXUcfHbMCa0eN8.js"></script>

  </head>
  <body class="default-view path-frontpage node--type-landing-page">

    <a href="#main-content" class="visually-hidden focusable" tabindex="1">
      Skip to main content
    </a>
    <noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-TD3BKV" height="0" width="0"></iframe></noscript>
    <container>
<div id="page-wrapper">
  <div id="page" class="homepage">

    <section role="header">
      <div class="header-content">
        <div id="global-header">
    
<div id="block-digitalgovsearch" class="block global-header-digitalgov-search">
  
    
        <div class="body"><div class="hide-for-small" id="global-search">
<form accept-charset="UTF-8" action="//secsearch.sec.gov/search" class="clearfix" id="global-search-form" method="get" name="form_iQueryForm">
<fieldset><legend></legend> <label class="overlabel" for="global-search-box" style="visibility: visible;">Search SEC.gov</label> <input name="utf8" type="hidden" value="?" /> <input class="affiliate" name="affiliate" type="hidden" value="secsearch" /> <input aria-autocomplete="list" aria-haspopup="true" autocomplete="off" class="usagov-search-autocomplete ui-autocomplete-input" id="global-search-box" name="query" role="textbox" tabindex="4" title="Search for" type="text" /> <span aria-hidden="true" class="button-label fa fa-search"> </span><input class="global-search-button" tabindex="5" title="Go" type="submit" value="" /></fieldset>
</form>

<p class="options"><a class="option-link" href="http://www.sec.gov/edgar/searchedgar/companysearch.html" tabindex="6">Company Filings</a> | <a class="option-link" href="http://www.sec.gov/search/search.htm" tabindex="7">More Search Options</a></p>
</div>
</div>
  </div>
<div id="block-secgov-branding" class="site-branding block system_branding_block">
  
    
  
    <div class="banner-seal">
    <a href="/" title="SEC Emblem" rel="home" tabindex="2">
      <img src="/files/sec-logo.png" alt="SEC Emblem" />
    </a>
  </div>
  
    <div class="banner-org-name">
      <a href="/" title="U.S. Securities and Exchange Commission" rel="home" tabindex="3">U.S. Securities and Exchange Commission</a>
  </div>
   

</div>

  </div>

      </div>
      <div id="global-navigation">
          <div class="navigation-wrapper">
    <div id="block-secgov-main-menu" class="block main">
  
    
    
        <div class="menu-toggle-target menu-toggle-target-show" id="show-block-secgov-main-menu"></div>
    <div class="menu-toggle-target" id="hide-block-secgov-main-menu"></div>

    <a class="menu-toggle" href="#show-block-secgov-main-menu">Show &mdash; Main navigation</a>

    <a class="menu-toggle menu-toggle--hide" href="#hide-block-secgov-main-menu">Hide &mdash; Main navigation</a>
    
              <ul id="main-menu">
                          <li >
                <a href="/about.shtml" title="About">About</a>
                                        <ul>
                          <li>
                <a href="/Article/whatwedo.html" title="What We Do">What We Do</a>
                      </li>
                    <li>
                <a href="/Article/about-commissioners.html" title="Commissioners">Commissioners</a>
                      </li>
                    <li>
                <a href="/answers/about-lawsshtml.html" title="Securities Laws">Securities Laws</a>
                      </li>
                    <li>
                <a href="/about/sec-docket.shtml" title="SEC Docket">SEC Docket</a>
                      </li>
                    <li>
                <a href="/reports" title="Reports and Publications">Reports and Publications</a>
                      </li>
                    <li>
                <a href="/careers" title="Careers">Careers</a>
                      </li>
                    <li>
                <a href="/contact-information/sec-directory" title="Contact">Contact</a>
                      </li>
        </ul>
  
              </li>
                    <li >
                <a href="/divisions.shtml" title="Divisions &amp; Offices">Divisions &amp; Offices</a>
                                        <ul>
                          <li>
                <a href="/divisions/corpfin.shtml" title="Corporation Finance">Corporation Finance</a>
                      </li>
                    <li>
                <a href="/divisions/enforce.shtml" title="Enforcement">Enforcement</a>
                      </li>
                    <li>
                <a href="/investment" title="Investment Management">Investment Management</a>
                      </li>
                    <li>
                <a href="/divisions/riskfin.shtml" title="Economic and Risk Analysis">Economic and Risk Analysis</a>
                      </li>
                    <li>
                <a href="/divisions/marketreg.shtml" title="Trading and Markets">Trading and Markets</a>
                      </li>
                    <li>
                <a href="/alj" title="Office of Administrative Law Judges">Office of Administrative Law Judges</a>
                      </li>
                    <li>
                <a href="/about/offices/ocie.shtml" title="Office of Compliance Inspections and Examinations">Office of Compliance Inspections and Examinations</a>
                      </li>
                    <li>
                <a href="/page/sec-regional-offices" title="Regional Offices">Regional Offices</a>
                      </li>
                    <li>
                <a href="/divisions.shtml" title="All Divisions and Offices">All Divisions and Offices</a>
                      </li>
        </ul>
  
              </li>
                    <li >
                <a href="https://www.sec.gov/litigation.shtml" title="Enforcement">Enforcement</a>
                                        <ul>
                          <li>
                <a href="/litigation/litreleases.shtml" title="Litigation Releases">Litigation Releases</a>
                      </li>
                    <li>
                <a href="/litigation/admin.shtml" title="Administrative Proceedings">Administrative Proceedings</a>
                      </li>
                    <li>
                <a href="/litigation/opinions.shtml" title="Opinions and Adjudicatory Orders">Opinions and Adjudicatory Orders</a>
                      </li>
                    <li>
                <a href="/divisions/enforce/friactions.shtml" title="Accounting and Auditing">Accounting and Auditing</a>
                      </li>
                    <li>
                <a href="/litigation/suspensions.shtml" title="Trading Suspensions">Trading Suspensions</a>
                      </li>
                    <li>
                <a href="/news/newsroom/howinvestigationswork.html" title="How Investigations Work">How Investigations Work</a>
                      </li>
        </ul>
  
              </li>
                    <li >
                <a href="/rules.shtml" title="Regulation">Regulation</a>
                                        <ul>
                          <li>
                <a href="/rules/rulemaking-index.shtml" title="Rulemaking Index">Rulemaking Index</a>
                      </li>
                    <li>
                <a href="/rules/proposed.shtml" title="Proposed Rules">Proposed Rules</a>
                      </li>
                    <li>
                <a href="/rules/final.shtml" title="Final Rules">Final Rules</a>
                      </li>
                    <li>
                <a href="/rules/interim-final-temp.shtml" title="Interim Final Temporary Rules">Interim Final Temporary Rules</a>
                      </li>
                    <li>
                <a href="/rules/other.shtml" title="Other Orders and Notices">Other Orders and Notices</a>
                      </li>
                    <li>
                <a href="/rules/sro.shtml" title="Self-Regulatory Organizations">Self-Regulatory Organizations</a>
                      </li>
                    <li>
                <a href="/interps.shtml" title="Staff Interpretations">Staff Interpretations</a>
                      </li>
        </ul>
  
              </li>
                    <li >
                <a href="/investor" title="Education">Education</a>
                                        <ul>
                          <li>
                <a href="https://investor.gov/" title="Investor.gov">Investor.gov</a>
                      </li>
                    <li>
                <a href="/check-your-investment-professional" title="Check Your Financial Professional">Check Your Financial Professional</a>
                      </li>
                    <li>
                <a href="/investor/alerts" title="Investor Alerts and Bulletins">Investor Alerts and Bulletins</a>
                      </li>
                    <li>
                <a href="/answers.shtml" title="Fast Answers">Fast Answers</a>
                      </li>
                    <li>
                <a href="/complaint/select.shtml" title="File a Tip or Complaint">File a Tip or Complaint</a>
                      </li>
                    <li>
                <a href="/investor/pubs.shtml" title="Publications">Publications</a>
                      </li>
        </ul>
  
              </li>
                    <li >
                <a href="/edgar.shtml" title="Filings">Filings</a>
                                        <ul>
                          <li>
                <a href="/edgar/searchedgar/webusers.htm" title="EDGAR Search Tools">EDGAR Search Tools</a>
                      </li>
                    <li>
                <a href="/edgar/searchedgar/companysearch.html" title="Company Filing Search">Company Filing Search</a>
                      </li>
                    <li>
                <a href="/oiea/Article/edgarguide.html" title="How to Search EDGAR">How to Search EDGAR</a>
                      </li>
                    <li>
                <a href="/fast-answers/answerspublicdocshtm.html" title="Requesting Public Documents">Requesting Public Documents</a>
                      </li>
                    <li>
                <a href="/forms" title="Forms List">Forms List</a>
                      </li>
                    <li>
                <a href="/page/infoedgarshtml" title="Information for Filers">Information for Filers</a>
                      </li>
                    <li>
                <a href="/edgar/aboutedgar.htm" title="About EDGAR">About EDGAR</a>
                      </li>
        </ul>
  
              </li>
                    <li >
                <a href="/news" title="News">News</a>
                                        <ul>
                          <li>
                <a href="/news/pressreleases" title="Press Releases">Press Releases</a>
                      </li>
                    <li>
                <a href="/news/statements" title="Public Statements">Public Statements</a>
                      </li>
                    <li>
                <a href="/news/speeches" title="Speeches">Speeches</a>
                      </li>
                    <li>
                <a href="/news/testimony" title="Testimony">Testimony</a>
                      </li>
                    <li>
                <a href="/spotlight" title="Spotlight Topics">Spotlight Topics</a>
                      </li>
                    <li>
                <a href="/news/whatsnew/wn-today.shtml" title="What&#039;s New">What&#039;s New</a>
                      </li>
                    <li>
                <a href="/news/upcoming-events" title="Upcoming Events">Upcoming Events</a>
                      </li>
                    <li>
                <a href="https://www.sec.gov/news/webcasts.shtml" title="Webcasts">Webcasts</a>
                      </li>
                    <li>
                <a href="/news/sec-videos" title="SEC Videos">SEC Videos</a>
                      </li>
                    <li>
                <a href="/news/media-gallery" title="Media Gallery">Media Gallery</a>
                      </li>
        </ul>
  
              </li>
        </ul>
  

  
</div>
<nav role="navigation" aria-labelledby="block-secgov-account-menu-menu" id="block-secgov-account-menu">
            
  <h2 class="visually-hidden">User account menu</h2>
  

        
              <ul id="user-menu" role="menubar" aria-hidden="false">
        
            <li class="login" role="menuitem">
              <a href="/user/login" data-drupal-link-system-path="user/login">Log in</a>
              </li>


        </ul>
  


  </nav>

  </div>

        <div class="mobile-menu"><span class="fa fa-navicon"></span></div>
      </div>
    </section>

          <div class="highlighted">
        <aside class="message section clearfix" role="complementary">
            <div>
    

  </div>

        </aside>
      </div>
       
    <section role="content">
      <a id="main-content" tabindex="-1"></a>

      <div id="sidebar-first" class="sidebar">
        <a class="left-nav-menu"><span class="fa fa-navicon"></span></a>
        <aside class="local-nav" role="complementary">
          
              <ul class="mobile-nav">
              <li>
        <a href="/about">About</a>
                                <ul class="submenu">
              <li>
        <a href="/Article/whatwedo.html" data-drupal-link-system-path="node/91891">What We Do</a>
              </li>
          <li>
        <a href="/Article/about-commissioners.html" data-drupal-link-system-path="node/91916">Commissioners</a>
              </li>
          <li>
        <a href="/answers/about-lawsshtml.html" data-drupal-link-system-path="node/91696">Securities Laws</a>
              </li>
          <li>
        <a href="/about/sec-docket.shtml">SEC Docket</a>
              </li>
          <li>
        <a href="/reports" data-drupal-link-system-path="reports">Reports and Publications</a>
              </li>
          <li>
        <a href="/careers" data-drupal-link-system-path="node/41311">Careers</a>
              </li>
          <li>
        <a href="/contact.shtml">Contact</a>
              </li>
        </ul>
  
              </li>
          <li>
        <a href="/divisions">Divisions</a>
                                <ul class="submenu">
              <li>
        <a href="/corpfin">Corporation Finance</a>
              </li>
          <li>
        <a href="/enforce">Enforcement</a>
              </li>
          <li>
        <a href="/investment" data-drupal-link-system-path="node/38806">Investment Management</a>
              </li>
          <li>
        <a href="/dera" data-drupal-link-system-path="node/21296">Economic and Risk Analysis</a>
              </li>
          <li>
        <a href="/tm">Trading and Markets</a>
              </li>
          <li>
        <a href="/ocie" data-drupal-link-system-path="node/41211">National Exam Program</a>
              </li>
          <li>
        <a href="/divisions.shtml" data-drupal-link-system-path="node/91856">All Divisions and Offices</a>
              </li>
        </ul>
  
              </li>
          <li>
        <a href="/litigation">Enforcement</a>
                                <ul class="submenu">
              <li>
        <a href="/litigation/litreleases.shtml">Litigation Releases</a>
              </li>
          <li>
        <a href="/litigation/admin.shtml">Administrative Proceedings</a>
              </li>
          <li>
        <a href="/litigation/opinions.shtml">Opinions and Adjudicatory Orders</a>
              </li>
          <li>
        <a href="/divisions/enforce/friactions.shtml">Accounting and Auditin</a>
              </li>
          <li>
        <a href="/litigation/suspensions.shtml">Trading Suspensions</a>
              </li>
          <li>
        <a href="/news/newsroom/howinvestigationswork.html">How Investigations Work</a>
              </li>
          <li>
        <a href="/page/aljsectionlanding" data-drupal-link-system-path="node/3716">Administrative Law Judges</a>
              </li>
        </ul>
  
              </li>
          <li>
        <a href="/rules">Regulation</a>
                                <ul class="submenu">
              <li>
        <a href="/rules/rulemaking-index.shtml">Rulemaking Index</a>
              </li>
          <li>
        <a href="/rules/proposed.shtml">Proposed Rules</a>
              </li>
          <li>
        <a href="/rules/final.shtml">Final Rules</a>
              </li>
          <li>
        <a href="/rules/other.shtml">Other Orders and Notices</a>
              </li>
          <li>
        <a href="/rules/interim-final-temp.shtml">Interim Final Rules</a>
              </li>
          <li>
        <a href="/rules/other.shtml">Other Orders and Notices</a>
              </li>
          <li>
        <a href="/rules/sro.shtml">Self Regulatory Organizations</a>
              </li>
          <li>
        <a href="/interps.shtml">Staff Interpretations</a>
              </li>
        </ul>
  
              </li>
          <li>
        <a href="/investor">Education</a>
                                <ul class="submenu">
              <li>
        <a href="http://investor.gov/">Investor.gov</a>
              </li>
          <li>
        <a href="/reportspubs/investor-publications/investor-brokershtm.html" data-drupal-link-system-path="node/89386">Check Out a Broker or Advisor</a>
              </li>
          <li>
        <a href="/investor/alerts" data-drupal-link-system-path="investor/alerts">Investor Alerts and Bulletins</a>
              </li>
          <li>
        <a href="/fast-answers" data-drupal-link-system-path="fast-answers">Fast Answers</a>
              </li>
          <li>
        <a href="/complaint/select.shtml" data-drupal-link-system-path="node/111826">File a Tip or Complaint</a>
              </li>
          <li>
        <a href="/investor/pubs.shtml">Publications</a>
              </li>
        </ul>
  
              </li>
          <li>
        <a href="/edgar.shtml" data-drupal-link-system-path="node/91901">Filings</a>
                                <ul class="submenu">
              <li>
        <a href="/edgar/searchedgar/webusers.htm" data-drupal-link-system-path="node/91871">EDGAR Search Tools</a>
              </li>
          <li>
        <a href="/edgar/searchedgar/companysearch.html">Company Filings Search</a>
              </li>
          <li>
        <a href="/oiea/Article/edgarguide.html" data-drupal-link-system-path="node/91976">How to Search EDGAR</a>
              </li>
          <li>
        <a href="/fast-answers/answerspublicdocshtm.html" data-drupal-link-system-path="node/90616">Requesting Public Documents</a>
              </li>
          <li>
        <a href="/about/forms/secforms.htm">Forms List</a>
              </li>
          <li>
        <a href="/page/infoedgarshtml" data-drupal-link-system-path="node/96001">Information for Filers</a>
              </li>
          <li>
        <a href="/edgar/aboutedgar.htm">About EDGAR</a>
              </li>
        </ul>
  
              </li>
          <li>
        <a href="/news">News</a>
                                <ul class="submenu">
              <li>
        <a href="/news/pressreleases" data-drupal-link-system-path="news/pressreleases">Press Releases</a>
              </li>
          <li>
        <a href="/news/statements" data-drupal-link-system-path="news/statements">Public Statements</a>
              </li>
          <li>
        <a href="/speeches">Speeches</a>
              </li>
          <li>
        <a href="/news/testimony" data-drupal-link-system-path="news/testimony">Testimony</a>
              </li>
          <li>
        <a href="/spotlight" data-drupal-link-system-path="node/96191">Spotlight Topics</a>
              </li>
          <li>
        <a href="/news/whatsnew/wn-today.shtml">What&#039;s New</a>
              </li>
          <li>
        <a href="/news/upcoming-events" data-drupal-link-system-path="node/40730">Events</a>
              </li>
          <li>
        <a href="/news/media-gallery" data-drupal-link-system-path="node/41986">Media Gallery</a>
              </li>
          <li>
        <a href="/news/webcasts.shtml">Webcasts</a>
              </li>
        </ul>
  
              </li>
        </ul>
  


          <div class="clearfix"></div>
          <div id="mobile-search" >
  <form accept-charset="UTF-8" action="//secsearch.sec.gov/search" class="clearfix" id="mobile-search-form" method="get" name="form_iQueryForm" data-drupal-form-fields="global-search-box">
    <fieldset>
      <legend></legend><div class="search-box-container">
      <label class="overlabel" for="global-search-box" style="visibility: visible;">Search SEC.gov</label>
      <input name="utf8" type="hidden" value="?">
      <input class="affiliate" name="affiliate" type="hidden" value="secsearch">
      <input aria-autocomplete="list" aria-haspopup="true" autocomplete="off" class="usagov-search-autocomplete ui-autocomplete-input" id="mobile-search-box" name="query" role="textbox" tabindex="4" title="Search for" type="text">
      <span class="button-label fa fa-search"> </span>
      <input class="global-search-button" tabindex="5" title="Go" type="submit" value=""></div>
    </fieldset>
  </form>
  <p class="options"><a href="http://www.sec.gov/edgar/searchedgar/companysearch.html" tabindex="6">Company Filings</a> | <a href="http://www.sec.gov/search/search.htm" tabindex="7">More Search Options</a></p>
</div>        </aside>
      </div>
      
              
      
            <div id="home">
          <div class="main-content">
    <div id="block-secgov-content">
  
    
      
<article data-history-node-id="2431" class="node node--type-landing_page node--view-mode-full clearfix">
  
    

  <div>
    <div class="panel-display panel-1col clearfix" >

                                  <section id="alert" class="hp-section">
                      <div class="block-region-alert"><div class="views-element-container block site_alerts-view_alerts_block_homepage">
  
    
      <div>
<div class="view view-site-alerts view-id-site_alerts view-display-id-view_alerts_block_homepage js-view-dom-id-1e42f269ab6e1dfc8968bb51db4e2a3c2d2b1915c6e33c69f9bcecdee6e97789">
  
  
  

  
    
  
  


        
        
  
  
  
    <div class="homepage-alert Info promote view-row-count-1 view-row-first">
      <div><div class="alert-title">Information for Longfin Corp. Investors</div></div><div><div class="alert-body"><p>For details, <a href="/enforce/information-longfin-investors">read the article here</a>.</p>
</div></div>
    </div>

  

  
    
  
    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
</div>
                  </section>
            
  	<section id="hero" class="hero">
	<div class="block-region-hero"><div class="views-element-container block homepage_hero-block_1">
  
    
      <div>
<div class="hp-hero view view-homepage-hero view-id-homepage_hero view-display-id-block_1 js-view-dom-id-dd4f0ef0cf9b9f697a375c2a59a2d3feaf6d333bdce29501d6c83f37993e3544">
  
  
  

  
    
  
  
<div>
    
<div id="flexslider-1" class="flexslider optionset-homepage-hero">
 
<ul class="slides">
    
<li>
    <div class="views-field views-field-body"><div class="field-content"><style type="text/css">
<!--/*--><![CDATA[/* ><!--*/
.slide-content-box {margin:0;}
@media only screen and (min-width: 768px) and (max-width: 1440px) {
  .slide-content-box {margin: 3rem 0 0 3rem;}
}
@media only screen and (min-width: 1440px) {
  .slide-content-box {margin: 8% 0 0 25%;}
}

/*--><!]]>*/
</style><div id="slide-1"><img alt="We are the Investor's Advocate" data-entity-type="file" src="/files/investor_advocate.jpg.jpeg" /><div class="slide-content-box">
<div class="slide-headline"><span class="headline-1">WE ARE THE </span><span class="headline-2">INVESTOR'S ADVOCATE</span></div>

<div class="slide-description">
<div class="slide-description-text">
<p>The SEC protects investors, promotes fairness in the securities markets, and shares information about companies and investment professionals to help investors make informed decisions and invest with confidence.</p>
</div>
</div>
</div>
</div></div></div>
    </li>
</ul>
</div>

</div>

  
    
  
    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
<div class="block sec_mission_block">
  <div id="sec-mission">
      <div class="hp-content">
          <div class="hp-content-item odd">
          <a href="#section-2" title="Go to We Inform and Protect Investors">
              <div class="hp-content-icon">
                  <img alt="Icon: We Inform and Protect Investors" src="/themes/custom/secgov/images/homepage/inform-icon-2x.png" />
              </div>
              <div class="hp-content-title">We Inform and Protect Investors</div>
          </a>
          </div>

          <div class="hp-content-item even">
          <a href="#section-3" title="Go to We Facilitate Capital Formation">
              <div class="hp-content-icon">
                  <img alt="Icon: We Facilitate Capital Formation" src="/themes/custom/secgov/images/homepage/cap-formation.png" />
              </div>
              <div class="hp-content-title">We Facilitate Capital Formation</div>
          </a>
          </div>

          <div class="hp-content-item odd">
          <a href="#section-4" title="Go to We Enforce Federal Securities Laws">
              <div class="hp-content-icon">
                  <img alt="Icon: We Enforce Federal Securities Laws" src="/themes/custom/secgov/images/homepage/enforce-icon-2x.png" />
              </div>
              <div class="hp-content-title">We Enforce Federal Securities Laws</div>
          </a>
          </div>

          <div class="hp-content-item even">
          <a href="#section-5" title="Go to We Regulate Securities Markets">
              <div class="hp-content-icon">
                  <img alt="Icon: We Regulate Securities Markets" src="/themes/custom/secgov/images/homepage/regulate-securities.png" />
              </div>
              <div class="hp-content-title">We Regulate Securities Markets</div>
          </a>
          </div>

          <div class="hp-content-item last odd">
          <a href="#section-6" title="Go to We Provide Data">
              <div class="hp-content-icon">
                  <img alt="Icon: We Provide Data" src="/themes/custom/secgov/images/homepage/data-icon-2x.png" />
              </div>
              <div class="hp-content-title">We Provide Data</div>
          </a>
          </div>

          <div class="sec-mission-footer">
              <p class="sec-mission-description">
                  <span class="emphasis-1" style="font-size: 18px">EDGAR |</span>
                  <span class="emphasis-2" style="font-size: 14px;">Company Filings -</span> Free access to 21 million filings.
              </p>
              <div id="edgar">
                <form id="edgar-search" action="/cgi-bin/browse-edgar" method="get" name="companysearch">
                    <div class="row">
                        <div class="large-12 columns">
                            <div class="row collapse">
                              <label for="company-name" class="show-for-sr"><em>Company Name</em></label>
                              <div class="small-11 medium-11 large-11 columns">
                                <span class="twitter-typeahead" style="position: relative; display: inline-block;">
                                  <input id="company-name" name="company" title="Search For" type="text" value="Name or Ticker" class="tt-input" autocomplete="off" spellcheck="false" dir="auto" style="position: relative; vertical-align: top;">
                                  <pre aria-hidden="true" style="position: absolute; visibility: hidden; white-space: pre; font-family: Helvetica, sans-serif; font-size: 14.000040054321289px; font-style: normal; font-variant-ligatures: no-common-ligatures; font-variant-numeric: normal; font-variant-caps: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-east-asian: normal; font-weight: normal; word-spacing: 0px; letter-spacing: normal; text-indent: 0px; text-rendering: auto; text-transform: none;"></pre>
                                  <div class="tt-menu" style="position: absolute; top: 100%; left: 0px; z-index: 100; display: none; width: 292px;">
                                    <div class="tt-dataset tt-dataset-companies"></div>
                                  </div>
                                </span>
                              </div>

                              <div class="small-1 medium-1 large-1 columns">
                                <button id="edgar-search-button" type="submit" class="button postfix table-block">
                                  <span class="show-for-sr">Search</span>
                                  <i class="svg-icon svg-icon-sm svg-icon-box-md icon-search cell-block vcenter text-center">c</i>
                                </button>
                              </div>

                              <div class="edgar-search-hidden">
                                <input value="contains" name="match" type="hidden">
                                <input value="getcompany" name="action" type="hidden">
                              </div>
                            </div>
                        </div>
                    </div>
                </form>
                <form class="companySearchForm" id="fast-search" method="get" action="https://www.sec.gov/cgi-bin/browse-edgar">
                    <div class="row">
                        <div class="large-12 columns">
                            <div class="row collapse">
                              <label for="cik" class="show-for-sr"><em>Ticker or CIK</em></label>
                              <div class="small-11 medium-11 large-11 columns">
                                <input id="cik" name="CIK" title="Ticker or CIK" type="text" value="Ticker or CIK">
                              </div>

                              <div class="small-1 medium-1 large-1 columns">
                                <button id="cik_find" type="submit" class="button postfix table-block">
                                  <span class="show-for-sr">Search</span>
                                  <i class="svg-icon svg-icon-sm svg-icon-box-md icon-search cell-block vcenter text-center">c</i>
                                </button>
                              </div>

                              <div class="edgar-search-hidden">
                                <input type="hidden" name="action" value="getcompany">
                                <input type="hidden" name="owner" value="exclude">
                              </div>
                            </div>
                        </div>
                    </div>
                </form>
              </div>
          </div>
      </div>
  </div>
</div>
</div>
	</section>
  
  <section id="section-1" class="hp-section odd-row">
  	<div class="panel-panel panel-col">
    	<h2></h2>
    	<div class="column colspan-8"><div class="block-region-section-1-left"><div class="views-element-container block homepage_featured_stories-sec_stories">
  
    
      <div>
<div class="featured-content view view-homepage-featured-stories view-id-homepage_featured_stories view-display-id-sec_stories js-view-dom-id-84c75e7ac150901b7169829cb5f5a92a184b06e0430c9ae2ba94aa88521dbe0e">
  
  
  

      <header>
      <h3>SEC Stories</h3>
    </header>
  
    
  
      <div class="views-view-grid horizontal cols-2 clearfix">
            <div class="sec-stories-rows views-row clearfix row-1">
                  <div class="sec-stories-col views-col col-1">
            <div class="views-field views-field-field-featured-graphic"><div class="field-content">  <a href="/page/miami-regional-office-outreach-local-high-schools">  <img class="image-style-featured-graphic" src="/files/styles/featured_graphic/public/2018-04/highschool-outreach-thumbnail.jpg?itok=6f0f3do1" width="320" height="217" alt="highschool outreach" typeof="foaf:Image" />

</a>
</div></div><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
      <a href="/page/miami-regional-office-outreach-local-high-schools" hreflang="en">Miami Regional Office Outreach to Local High Schools </a>
  </div></div><div class="views-field views-field-field-alternate-title-secarticle"><div class="field-content"></div></div><div class="views-field views-field-field-teaser-text"><div class="field-content"></div></div><div class="views-field views-field-views-ifempty"><span class="field-content featured-content-teaser">It’s never too early to learn about personal finance. In support of April’s National Financial Capability Month, the SEC staff is helping to educate high school students about saving and investing.</span></div>
          </div>
                  <div class="sec-stories-col views-col col-2">
            <div class="views-field views-field-field-featured-graphic"><div class="field-content">  <a href="/page/sec-holocaust-remembrance-day">  <img class="image-style-featured-graphic" src="/files/styles/featured_graphic/public/2018-04/holocaust-thumbnail_0.jpg?itok=Rg9p4NGw" width="320" height="217" alt=" Holocaust Remembrance Day" typeof="foaf:Image" />

</a>
</div></div><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
      <a href="/page/sec-holocaust-remembrance-day" hreflang="en">SEC Holocaust Remembrance Day</a>
  </div></div><div class="views-field views-field-field-alternate-title-secarticle"><div class="field-content"></div></div><div class="views-field views-field-field-teaser-text"><div class="field-content"></div></div><div class="views-field views-field-views-ifempty"><span class="field-content featured-content-teaser">The SEC was privileged to host concentration camp survivor Rubin Sztajer at an event in honor of Holocaust Remembrance Day.</span></div>
          </div>
              </div>
      </div>

  
    
  
    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
<div class="views-element-container block featured_video-block_2">
  
    
      <div>
<div class="hp-featured-video view view-featured-video view-id-featured_video view-display-id-block_2 js-view-dom-id-48216c544c74a202710bd3fc60476045e9d8e11ca2169f1c5479bcab73cb6645">
  
  
  

      <header>
      <h3>Featured Video</h3>
    </header>
  
    
  
  


        
        
  
  
  
    <div class="views-row promote view-row-count-1 view-row-first">
      <span class="views-field views-field-field-video"><span class="field-content"><span class="field-content-video"><a href="/news/sec-videos/investorgov-exposed" hreflang="en">  <img class="image-style-featured-video" src="/files/styles/featured_video_image/public/video_thumbnails/a4KSyymwavM.jpg?itok=vmf36lTz" width="320" height="207" alt="" typeof="Image" />

</a></span>
<span class="field-content-runtime"></span>
</span></span><div class="views-field views-field-field-display-title"><h3 class="field-content">
      	  
      <a href="/news/sec-videos/investorgov-exposed" hreflang="en">Investor.gov&#039;s new PSA: &quot;Exposed&quot;</a>
  </h3></div><div class="views-field views-field-body"><div class="field-content"><p>Most fraudsters aren’t this easy to spot. Find out if you’re dealing with a registered investment professional with a free simple search at <a href="https://www.investor.gov">Investor.gov</a>.</p>
</div></div>
    </div>

  

  
    
  
    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
<div class="views-element-container block homepage_featured_spotlight-spotlight_topics">
  
    
      <div>
<div class="featured-content view view-homepage-featured-spotlight view-id-homepage_featured_spotlight view-display-id-spotlight_topics js-view-dom-id-8a4571c0ead5f0899c9d5ccb6c409814392f1d90520414808aebb221eb310907">
  
  
  

      <header>
      <h3>Spotlight On</h3>
    </header>
  
    
  
  


        
        
  
  
  
    <div class="views-row view-row-count-1 view-row-first">
      <div class="views-field views-field-field-featured-graphic"><div class="field-content featured-graphic">  <a href="/check-your-investment-professional">  <img class="image-style-featured-graphic" src="/files/styles/featured_graphic/public/2018-04/check-professional-thumbnail.jpg?itok=kNPKOwZl" width="320" height="217" alt="Check out Your Investment Professional Graphic " typeof="foaf:Image" />

</a>
</div></div><div class="views-field views-field-title"><h3 class="field-content"><a href="/check-your-investment-professional" hreflang="en">Check Your Investment Professional</a></h3></div><div class="views-field views-field-views-ifempty"><span class="field-content featured-content-teaser">Do you know who you are investing with? Check out this free search tool and find information about individuals that have been named in SEC court actions or administrative proceedings and had judgments or orders issued against them.</span></div>
    </div>

  

  
    
  <div class="more-link"><a href="/spotlight">More Spotlight Topics</a></div>

    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
</div></div>
    	<div class="column colspan-4 last"><div class="block-region-section-1-right"><div class="views-element-container block homepage_latest_news-homepage">
  
    
      <div>
<div class="view view-homepage-latest-news view-id-homepage_latest_news view-display-id-homepage js-view-dom-id-c63b1e8e0814052431a06a69e22ba522523faceee56fdd69a8fd9f9b9987eff3">
  
  
  

      <header>
      <h3>Latest News</h3>
    </header>
  
    
  
  <div class="item-list">
  
  <ul>

          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
      <a href="/news/press-release/2018-78" hreflang="en">SEC Launches Additional Investor Protection Search Tool</a>
  </div></div><div class="views-field views-field-field-publish-date"><div class="field-content">    <time datetime="2018-05-02T16:01:05Z" class="datetime">May 2, 2018</time>

</div></div></li>
          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
      <a href="/news/press-release/2018-75" hreflang="en">SEC Enforcement Division Issues FAQs for Share Class Selection Disclosure Initiative</a>
  </div></div><div class="views-field views-field-field-publish-date"><div class="field-content">    <time datetime="2018-05-01T18:00:00Z" class="datetime">May 1, 2018</time>

</div></div></li>
          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
      <a href="/news/press-release/2018-73" hreflang="en">Panasonic Charged With FCPA and Accounting Fraud Violations</a>
  </div></div><div class="views-field views-field-field-publish-date"><div class="field-content">    <time datetime="2018-04-30T17:55:00Z" class="datetime">April 30, 2018</time>

</div></div></li>
          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
      <a href="/news/press-release/2018-71" hreflang="en">Altaba, Formerly Known as Yahoo!, Charged With Failing to Disclose Massive Cybersecurity Breach; Agrees To Pay $35 Million</a>
  </div></div><div class="views-field views-field-field-publish-date"><div class="field-content">    <time datetime="2018-04-24T15:30:00Z" class="datetime">April 24, 2018</time>

</div></div></li>
          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
      <a href="/news/press-release/2018-70" hreflang="en">SEC Charges Additional Defendant in Fraudulent ICO Scheme</a>
  </div></div><div class="views-field views-field-field-publish-date"><div class="field-content">    <time datetime="2018-04-20T17:35:00Z" class="datetime">April 20, 2018</time>

</div></div></li>
    
  </ul>

</div>

  
    
  
    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>

<div id="subscribe">
  <div class="panel">
    <h2>E-mail Updates</h2>
    <p>Sign up for emails that will deliver SEC News direct to your inbox.</p>
    <form accept-charset="UTF-8" action="https://public.govdelivery.com/accounts/USSEC/subscribers/qualify" id="GD-snippet-form" method="post" name="GD-snippet-form">
      <input name="utf8" type="hidden" value="?"><input name="authenticity_token" type="hidden" value="rNLpZE6ui1SUXb98DT0ck6yojFmsiphJS29lz62OQ/k=">
      <div class="row">
        <div class="row collapse">
          <label class="show-for-sr" for="email">E-mail Updates</label> <input id="email" name="email" onblur="if (this.value == '') {this.value = 'Email address'; this.style.color='#b1b1b1';} else if (this.value != '') {this.style.color='#000';}" onfocus="if(this.value == 'Email address') {this.value = ''; this.style.color='#000';}" title="Enter email address" type="text" value="Email address">
        </div>
      </div>
      <div class="row">
        <input class="form_button small button" name="commit" type="submit" value="Subscribe">
      </div>
    </form>
    <script type="text/javascript">
      //<![CDATA[
        var GOVDSNIPPET = function() {
          var form  = document.getElementById('GD-snippet-form');
          var typeSelect = form.getElementsByTagName('select')[0];
          var getStyleType = function(type) {
            return typeSelect.value === type ? 'block' : 'none';
          };
          var toggleType = function() {
            form.getElementsByTagName('li')[2].style.display = getStyleType('email');
            form.getElementsByTagName('li')[1].style.display = getStyleType('phone');
          };
          if (typeSelect.addEventListener) {
            typeSelect.addEventListener('change', toggleType);
          } else if (typeSelect.attachEvent)  {
            typeSelect.attachEvent('onchange', toggleType);
          }
        }();
      //]]>
    </script>
  </div>
</div>
</div></div>
  	</div>
  </section>

  <section id="section-2" class="hp-section even-row">
    <div class="panel-panel panel-col">
    	<h2><div class="block-region-section-2-title">
<div class="block homepage-section-2-title">
  
    
        <div class="body"><script type="text/javascript">
jQuery(function($) {
  $(document).ready(function() {
    $(".homepage_featured_content-we_inform_and_protect_investors a").each(function(i) {
      if ($(this).attr("href") == '/spotlight/affinity-fraud.shtml') {
        $(this).attr("href", "https://www.fbi.gov/news/stories/beware-of-affinity-fraud");
      }
    });
  });
});
</script>
<h2><a name="section2"></a>We Inform and Protect Investors</h2></div>
  </div>
</div></h2>
      <div class="column colspan-4"><div class="block-region-section-2-left">
<div class="block homepage-protect-your-money">
  
    
        <div class="body"><h3>Protect Your Money!</h3>

<p>Check out an investment professional's registration status and background at <a href="https://www.investor.gov">Investor.gov</a>.</p>

<p class="section-3-button"><a href="check-your-investment-professional">Check Your<br />
Investment<br />
Professional</a></p></div>
  </div>
<div class="views-element-container block fast_answers_view-block_2">
  
    
      <div>
<div class="fast-answers-day homepage-block view view-fast-answers-view view-id-fast_answers_view view-display-id-block_2 js-view-dom-id-5bc3d8460cfa1949435b3f5614268f471f97fe9c24d83fdcbcd790e5c2008e6a">
  
  
  

      <header>
      <h3>Learn more</h3>
    </header>
  
    
  
  <div class="item-list">
  
  <ul>

          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
    <a href="/fast-answers/answersadvancefeefraudhtm.html" hreflang="en">Advance Fee Fraud</a>
  </div></div></li>
          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
    <a href="/fast-answers/answersetfhtm.html" hreflang="en">Exchange-Traded Funds (ETFs)</a>
  </div></div></li>
          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
    <a href="/fast-answers/answers-form10khtm.html" hreflang="en">Form 10-K</a>
  </div></div></li>
          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
    <a href="/fast-answers/answersvarannhtm.html" hreflang="en">Variable Annuities</a>
  </div></div></li>
    
  </ul>

</div>

  
    
  
      <footer>
      <div class="more-link">
<a href="https://www.investor.gov">Before you invest, Investor.gov</a>
</div>
    </footer>
    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
</div></div>
      <div class="column colspan-8 last"><div class="block-region-section-2-right"><div class="views-element-container block investor_alerts_bulletins_list_page-block_2">
  
    
      <div>
<div class="investor-alerts-block dynamic-block view view-investor-alerts-bulletins-list-page view-id-investor_alerts_bulletins_list_page view-display-id-block_2 js-view-dom-id-f43d0230bb6910fc7a37511d003507ff96791cc690e70053c8f00c39ed0f9f75">
  
  
  

      <header>
      <h3>Investor Alerts & Bulletins</h3>
<p>The SEC's Office of Investor Education and Advocacy issues Investor Alerts & Bulletins as a service to investors. Investor Alerts typically warn investors about the latest investment frauds and scams. Investor Bulletins tend to educate investors about investment-related topics including the functions of the SEC.</p>
    </header>
  
    
  
  <div class="item-list">
  
  <ul>

          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
    <a href="/oiea/investor-alerts-and-bulletins/ia_ponziseniors" hreflang="en">Investor Alert: Ponzi Schemes Targeting Seniors</a>
  </div></div><div class="views-field views-field-field-publish-date"><div class="field-content">    <time datetime="2018-04-09T14:27:59Z" class="datetime">April 9, 2018</time>

</div></div></li>
          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
    <a href="/oiea/investor-alerts-and-bulletins/ia_helpbuystock" hreflang="en">Investor Alert: SEC Impersonators Pretend to Help Investors Buy Stock<br/>(Listen to Audio)</a>
  </div></div><div class="views-field views-field-field-publish-date"><div class="field-content">    <time datetime="2018-04-04T13:02:33Z" class="datetime">April 4, 2018</time>

</div></div></li>
          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
    <a href="/oiea/investor-alerts-bulletins/ib_selectpro.html" hreflang="en">Updated Investor Bulletin: Top Tips for Selecting a Financial Professional</a>
  </div></div><div class="views-field views-field-field-publish-date"><div class="field-content">    <time datetime="2018-04-03T10:08:08Z" class="datetime">April 3, 2018</time>

</div></div></li>
    
  </ul>

</div>

  
    
  <div class="more-link"><a href="/investor/alerts">More Investor Alerts &amp; Bulletins</a></div>

    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
<div class="views-element-container block homepage_featured_content-we_inform_and_protect_investors">
  
    
      <div>
<div class="featured-content view view-homepage-featured-content view-id-homepage_featured_content view-display-id-we_inform_and_protect_investors js-view-dom-id-2ea357ad0ab6ee2db03455030f31bc4e51a8fd6ce2d0aa8aded5b002fca7ea2c">
  
  
  

      <header>
      
    </header>
  
    
  
  


        
        
  
  
  
    <div class="views-row promote view-row-count-1 view-row-first">
      <div class="views-field views-field-field-featured-graphic"><div class="field-content featured-graphic">  <a href="/teachers">  <img class="image-style-featured-graphic" src="/files/styles/featured_graphic/public/2018-03/homepage-teacheroutreach.jpg?itok=t5SnFYS9" width="320" height="217" alt="Teacher Outreach" typeof="foaf:Image" />

</a>
</div></div><div class="views-field views-field-view-node"><h4 class="field-content featured-content-title"><a href="/teachers" hreflang="en">Teachers Investment Options </a></h4></div><div class="views-field views-field-views-ifempty"><span class="field-content featured-content-teaser">When it comes to saving for retirement, you have big decisions to make, and the SEC wants to help. The SEC offers tools and resources to help you learn more about the 403(b) and 457(b) retirement plans that are most often offered in public school districts.</span></div>
    </div>

  

  
    
  
    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
</div></div>
    </div>
  </section>

  <section id="section-3"class="hp-section odd-row">
    <div class="panel-panel panel-col">
      <h2><div class="block-region-section-3-title">
<div class="block homepage-section-3-title">
  
    
        <div class="body"><h2>We Facilitate Capital Formation</h2>
</div>
  </div>
</div></h2>
      <div class="column colspan-8"><div class="block-region-section-3-left"><div class="views-element-container block homepage_featured_content_we_facilitate_capital_formation-we_facilitate_capital_formation">
  
    
      <div>
<div class="featured-content view view-homepage-featured-content-we-facilitate-capital-formation view-id-homepage_featured_content_we_facilitate_capital_formation view-display-id-we_facilitate_capital_formation js-view-dom-id-d17362490de2cfd17b31130e6e8134ff15b7362221445181ced8ef0d6e92da5c">
  
  
  

  
    
  
      <div class="views-view-grid vertical cols-1 clearfix">
            <div class="views-col clearfix col-1" style="width: 100%;">
                  <div class="views-row row-1">
            <div class="views-field views-field-field-featured-graphic"><div class="field-content featured-graphic">  <a href="/smallbusiness">  <img class="image-style-featured-graphic" src="/files/styles/featured_graphic/public/2017-11/SMB-thumbnail.jpg.jpeg?itok=E-7yfxK6" width="320" height="178" alt="Small Business featured graphic" typeof="foaf:Image" />

</a>
</div></div><div class="views-field views-field-title"><span class="field-content"><h4><a href="/smallbusiness" hreflang="en">Small Business</a></h4></span></div><div class="views-field views-field-views-ifempty"><span class="field-content featured-content-teaser">Check out our new Small Biz site, with info to help companies that want to raise capital.</span></div>
          </div>
                  <div class="views-row row-2">
            <div class="views-field views-field-field-featured-graphic"><div class="field-content featured-graphic">  <a href="/spotlight/crowdfunding.shtml">  <img class="image-style-featured-graphic" src="/files/styles/featured_graphic/public/2017-07/crowdfunding-spotlight.png?itok=k-hLK9Y4" width="317" height="193" alt="Crowdfunding featured graphic" typeof="foaf:Image" />

</a>
</div></div><div class="views-field views-field-title"><span class="field-content"><h4><a href="/spotlight/crowdfunding.shtml" hreflang="en">Crowdfunding</a></h4></span></div><div class="views-field views-field-views-ifempty"><span class="field-content featured-content-teaser">Crowdfunding is an evolving method of raising money via the Internet to fund a variety of projects.</span></div>
          </div>
              </div>
      </div>

  
    
  
    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
</div></div>
      <div class="column colspan-4 last"><div class="block-region-section-3-right"><div class="views-element-container block homepage_recent_news_we_facilitate_capital_formation-recent_capital_formation_news">
  
    
      <div>
<div class="featured-content view view-homepage-recent-news-we-facilitate-capital-formation view-id-homepage_recent_news_we_facilitate_capital_formation view-display-id-recent_capital_formation_news js-view-dom-id-1c37b85bc25873082921178608a1bbbe8d65ec235476abacb77f7b59f636135e">
  
  
  

  
    
  
  <div class="item-list">
  
  <ul class="cap-formation">

          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
      <a href="/news/public-statement/annual-government-business-forum-small-business-capital-formation" hreflang="en">Remarks to the Annual Government-Business Forum on Small Business Capital Formation</a>
  </div></div><div class="views-field views-field-views-ifempty"><span class="field-content featured-content-teaser">Chairman Jay Clayton discusses SEC efforts to facilitate companies’ access to capital while protecting investors.</span></div></li>
          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
      <a href="/dera/staff-papers/economic-analyses/access-to-capital-and-market-liquidity-study-2017" hreflang="en">Access to Capital and Market Liquidity</a>
  </div></div><div class="views-field views-field-views-ifempty"><span class="field-content featured-content-teaser">This report to Congress includes an examination of initial public offerings and crowdfunding by small companies.</span></div></li>
    
  </ul>

</div>

  
    
  
    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
</div></div>
    </div>
  </section>

  <section id="section-4" class="hp-section even-row">
    <div class="panel-panel panel-col">
      <h2><div class="block-region-section-4-title">
<div class="block homepage-section-6-title">
  
    
        <div class="body"><h2>We Enforce Federal Securities Laws</h2></div>
  </div>
</div></h2>
      <div class="column colspan-4"><div class="block-region-section-4-left"><div class="block submit_a_tip_button_block">
  
    
      <div class="button-box"><a href="/complaint/select.shtml"><span class="svg-icon svg-icon-lg">b</span> <span class="description">Submit a Tip or<br />
File a Complaint</span></a></div>
  </div>
<div class="block administrative_proceedings_button_block">
  
    
      <div class="button-box"><a href="/litigation/apdocuments.shtml"><span class="svg-icon svg-icon-lg">a</span> <span class="description">Administrative<br />
Proceeding<br />Documents</span></a></div>
  </div>
<div class="views-element-container block homepage_featured_content-we_enforce_federal_securities_laws">
  
    
      <div>
<div class="featured-content view view-homepage-featured-content view-id-homepage_featured_content view-display-id-we_enforce_federal_securities_laws js-view-dom-id-54298f84128fe85c53b883e8219a2510872de1f6e68150e5b69b0cde75520061">
  
  
  

      <header>
      
    </header>
  
    
  
  


        
        
  
  
  
    <div class="views-row promote view-row-count-1 view-row-first">
      <div class="views-field views-field-field-featured-graphic"><div class="field-content featured-graphic">  <a href="/whistleblower">  <img class="image-style-featured-graphic" src="/files/styles/featured_graphic/public/2017-08/whistleblower-spotlight.png?itok=Wb-zmVw1" width="303" height="151" alt="Whistleblower graphic" typeof="foaf:Image" />

</a>
</div></div><div class="views-field views-field-view-node"><h4 class="field-content featured-content-title"><a href="/whistleblower" hreflang="en">Office of the Whistleblower</a></h4></div><div class="views-field views-field-views-ifempty"><span class="field-content featured-content-teaser">Submit a tip, learn about the program, or claim an award.</span></div>
    </div>

  

  
    
  
    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
</div></div>
      <div class="column colspan-8 last"><div class="block-region-section-4-right"><div class="block litigation_releases_block">
  
    
      <h2>Latest Federal Court Actions</h2><h3>Litigation Releases</h3><ul><li><a href="https://www.sec.gov/litigation/litreleases/2018/lr24134.htm">David A. Zimliki and Russel P. Schiefer</a><span>May 4, 2018</span></li><li><a href="https://www.sec.gov/litigation/litreleases/2018/lr24133.htm">Paul W. Smith</a><span>May 4, 2018</span></li><li><a href="https://www.sec.gov/litigation/litreleases/2018/lr24132.htm">Adam Tracy and Securities Compliance Group, Ltd.</a><span>May 3, 2018</span></li><li><a href="https://www.sec.gov/litigation/litreleases/2018/lr24131.htm">Shawn Carter</a><span>May 3, 2018</span></li><li><a href="https://www.sec.gov/litigation/litreleases/2018/lr24130.htm">Longfin Corp., et al.</a><span>May 3, 2018</span></li></ul><div class="more-link"><a href="//www.sec.gov/litigation/litreleases.shtml">More Litigation Releases</a></div>
  </div>
<div class="block administrative_proceedings_block">
  
    
      <h2>Latest Administrative Proceedings</h2><h3>Administrative Releases</h3><ul><li><a href="https://www.sec.gov/litigation/admin/2018/34-83176.pdf">Joseph A. Rubbo</a><span>May 4, 2018</span></li><li><a href="https://www.sec.gov/litigation/admin/2018/34-83173.pdf">Daniel H. Glick, CPA</a><span>May 4, 2018</span></li><li><a href="https://www.sec.gov/litigation/admin/2018/34-83172.pdf">Gray Financial Group, Inc., et al.</a><span>May 4, 2018</span></li><li><a href="https://www.sec.gov/litigation/admin/2018/33-10492.pdf">Shae Yatta Harper, Esq.</a><span>May 4, 2018</span></li><li><a href="https://www.sec.gov/litigation/admin/2018/34-83170.pdf">David T. Leboe, CPA</a><span>May 4, 2018</span></li></ul><div class="more-link"><a href="//www.sec.gov/litigation/admin.shtml">More Administrative Releases</a></div>
  </div>
</div></div>
    </div>
  </section>

  <section id="section-5" class="hp-section odd-row">
    <div class="panel-panel panel-col">
      <h2><div class="block-region-section-5-title">
<div class="block homepage-section-5-title">
  
    
        <div class="body"><h2>We Regulate Securities Markets</h2></div>
  </div>
</div></h2>
      <div class="column colspan-8"><div class="block-region-section-5-left">
<div class="block credit-rating-agencies-/-final-rules-combo-button">
  
    
        <div class="body"><div class="callout">
<div class="field-title" style="margin-top:0; padding-bottom:0;"><a href="https://www.sec.gov/ocr/reportspubs/annual-reports/2017-annual-report-on-nrsros.pdf"><img alt="People" data-entity-type="file" src="/sites/default/files/inline-images/people.png" /><br /><br />
CREDIT RATING AGENCIES</a></div>
</div>

<div class="callout">
<div class="field-title" style="margin-top:0; padding-bottom:0;"><a href="rules/final.shtml"><img alt="Notepad" data-entity-type="file" src="/sites/default/files/inline-images/notepad.png" /><br /><br />
VIEW FINAL RULES</a></div>
</div></div>
  </div>
<div class="views-element-container block homepage_featured_content-we_regulate_securities_markets">
  
    
      <div>
<div class="featured-content view view-homepage-featured-content view-id-homepage_featured_content view-display-id-we_regulate_securities_markets js-view-dom-id-7d96bd92d62db621e65579e805a00f4bf53fa266c42ad6349584b64434500ceb">
  
  
  

      <header>
      
    </header>
  
    
  
  


        
        
  
  
  
    <div class="views-row promote view-row-count-1 view-row-first">
      <div class="views-field views-field-field-featured-graphic"><div class="field-content featured-graphic">  <a href="/spotlight/cybersecurity">  <img class="image-style-featured-graphic" src="/files/styles/featured_graphic/public/2017-07/cybersecurity-featured-graphic.jpg?itok=Z4LxIEw0" width="300" height="193" alt="Cybersecurity featured graphic" typeof="foaf:Image" />

</a>
</div></div><div class="views-field views-field-view-node"><h4 class="field-content featured-content-title"><a href="/spotlight/cybersecurity" hreflang="en">Cybersecurity, the SEC and You</a></h4></div><div class="views-field views-field-views-ifempty"><span class="field-content featured-content-teaser">As markets grow more global and complex, so too are the threats to cybersecurity.</span></div>
    </div>

  

  
    
  
    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
</div></div>
      <div class="column colspan-4 last"><div class="block-region-section-5-right">
<div class="block homepage-recent-proposed-rules-text">
  
    
        <div class="body"><h3 class="field-content">Requests for Public Comment</h3>

<ul class="no-bullet">
	<li>
	<form action="/cgi-bin/ruling-comments" class="margin-0" method="post" style="margin-bottom: 0;"><a href="javascript:;" onclick="parentNode.submit();">Form CRS Relationship Summary; Amendments to Form ADV; Required Disclosures in Retail Communications and Restrictions on the use of Certain Names or Titles</a> <input name="ruling" type="hidden" value="S7-08-18" /> <input name="action" type="hidden" value="Show_Form" /> <input name="rule_path" type="hidden" value="/comments/s7-08-18" /> <input name="file_num" type="hidden" value="s7-08-18" /> <input name="title" type="hidden" value="Form CRS Relationship Summary; Amendments to Form ADV; Required Disclosures in Retail Communications and Restrictions on the use of Certain Names or Titles" /> (See <a href="/rules/proposed.shtml#34-83063">Release</a> and <a href="/comments/s7-08-18/s70818.htm">Comments</a>)</form>
	</li>
	<li>
	<form action="/cgi-bin/ruling-comments" class="margin-0" method="post" style="margin-bottom: 0;"><a href="javascript:;" onclick="parentNode.submit();">Proposed Commission Interpretation Regarding Standard of Conduct for Investment Advisers; Request for Comment on Enhancing Investment Adviser Regulation</a> <input name="ruling" type="hidden" value="S7-09-18" /> <input name="action" type="hidden" value="Show_Form" /> <input name="rule_path" type="hidden" value="/comments/s7-09-18" /> <input name="file_num" type="hidden" value="s7-09-18" /> <input name="title" type="hidden" value="Proposed Commission Interpretation Regarding Standard of Conduct for Investment Advisers; Request for Comment on Enhancing Investment Adviser Regulation" /> (See <a href="/rules/proposed/2018/ia-4889.pdf">Release</a> and <a href="/comments/s7-09-18/s70918.htm">Comments</a>)</form>
	</li>
	<li>
	<form action="/cgi-bin/ruling-comments" class="margin-0" method="post" style="margin-bottom: 0;"><a href="javascript:;" onclick="parentNode.submit();">Regulation Best Interest</a> <input name="ruling" type="hidden" value="S7-07-18" /> <input name="action" type="hidden" value="Show_Form" /> <input name="rule_path" type="hidden" value="/comments/s7-07-18" /> <input name="file_num" type="hidden" value="s7-07-18" /> <input name="title" type="hidden" value="Regulation Best Interest" /> (See <a href="/rules/proposed/2018/34-83062.pdf">Release</a> and <a href="/comments/s7-07-18/s70718.htm">Comments</a>)</form>
	</li>
	<li><a href="https://www.sec.gov/news/public-statement/statement-chairman-clayton-2017-05-31">Public Comments from Retail Investors and Other Interested Parties on Standards of Conduct for Investment Advisers and Broker-Dealers</a></li>
	<li>
	<form action="/cgi-bin/ruling-comments" class="margin-0" method="post" style="margin-bottom: 0;"><a href="javascript:;" onclick="parentNode.submit();">Inline XBRL Filing of Tagged Data</a> <input name="ruling" type="hidden" value="S7-03-17" /> <input name="action" type="hidden" value="Show_Form" /> <input name="rule_path" type="hidden" value="/comments/s7-03-17" /> <input name="file_num" type="hidden" value="s7-03-17" /> <input name="title" type="hidden" value="Inline XBRL Filing of Tagged Data" /> (See <a href="/rules/proposed/2017/33-10323.pdf">Release</a> and <a href="https://www.sec.gov/comments/s7-03-17/s70317.htm">Comments</a>)</form>
	</li>
	<li>
	<form action="/cgi-bin/ruling-comments" class="margin-0" method="post" style="margin-bottom: 0;"><a href="javascript:;" onclick="parentNode.submit();">Proposed Amendments to Exchange Act Rule 15c2-12</a> <input name="ruling" type="hidden" value="S7-01-17" /> <input name="action" type="hidden" value="Show_Form" /> <input name="rule_path" type="hidden" value="/comments/s7-01-17" /> <input name="file_num" type="hidden" value="s7-01-17" /> <input name="title" type="hidden" value="Proposed Amendments to Exchange Act Rule 15c2-12" /> (See <a href="/rules/proposed/2017/34-80130.pdf">Release</a> and <a href="https://www.sec.gov/comments/s7-01-17/s70117.htm">Comments</a>)</form>
	</li>
	<li>
	<form action="/cgi-bin/ruling-comments" class="margin-0" method="post" style="margin-bottom: 0;"><a href="javascript:;" onclick="parentNode.submit();">Possible Changes to Industry Guide 3</a> <input name="ruling" type="hidden" value="S7-02-17" /> <input name="action" type="hidden" value="Show_Form" /> <input name="rule_path" type="hidden" value="/comments/s7-02-17" /> <input name="file_num" type="hidden" value="s7-02-17" /> <input name="title" type="hidden" value="Possible Changes to Industry Guide 3" /> (See <a href="/rules/other/2017/33-10321.pdf">Release</a> and <a href="/comments/s7-02-17/s70217.htm">Comments</a>)</form>
	</li>
	<li>
	<form action="/cgi-bin/ruling-comments" class="margin-0" method="post" style="margin-bottom: 0;"><a href="javascript:;" onclick="parentNode.submit();">Universal Proxy</a> <input name="ruling" type="hidden" value="S7-24-16" /> <input name="action" type="hidden" value="Show_Form" /> <input name="rule_path" type="hidden" value="/comments/s7-24-16" /> <input name="file_num" type="hidden" value="s7-24-16" /> <input name="title" type="hidden" value="Universal Proxy" /> (See <a href="/rules/proposed/2016/34-79164.pdf">Release</a> and <a href="https://www.sec.gov/comments/s7-24-16/s72416.htm">Comments</a>)</form>
	</li>
	<li>
	<form action="/cgi-bin/ruling-comments" class="margin-0" method="post" style="margin-bottom: 0;"><a href="javascript:;" onclick="parentNode.submit();">Report on the Review of the Definition of "Accredited Investor"</a> <input name="ruling" type="hidden" value="4-692" /> <input name="action" type="hidden" value="Show_Form" /> <input name="rule_path" type="hidden" value="/comments/4-692" /> <input name="file_num" type="hidden" value="4-692" /> <input name="title" type="hidden" value="Report on the Review of the Definition of 'Accredited Investor'" /> (See <a href="/corpfin/reportspubs/special-studies/review-definition-of-accredited-investor-12-18-2015.pdf">Report</a> and <a href="/comments/4-692/4-692.shtml">Comments</a>)</form>
	</li>
</ul>

<div class="more-link"><a href="/rules/submitcomments.htm" title="More Public Comments">More Public Comments</a></div>
</div>
  </div>
</div></div>
    </div>
  </section>

  <section id="section-6" class="hp-section even-row">
    <div class="panel-panel panel-col">
      <h2><div class="block-region-section-6-title">
<div class="block homepage-section-4-title">
  
    
        <div class="body"><h2>We Provide Data</h2>
</div>
  </div>
</div></h2>
      <div class="column colspan-4"><div class="block-region-section-6-left"><div class="block developer_resources_block">
  
    
      <div class="developer">
          <h3>Developer Resources</h3>
          <p>Check out updates on the SEC open data program, including best practices that
          make it more efficient to download data.</p>
          <p class="xbrl-link-box"><a href="/developer">View Developer Resources</a></p>
        </div>
  </div>
</div></div>
      <div class="column colspan-8 last"><div class="block-region-section-6-right"><div class="views-element-container block data_list_page-block_1">
  
    
      <div>
<div class="data-list article-list view view-data-list-page view-id-data_list_page view-display-id-block_1 js-view-dom-id-89f0318fb3a3dd6e66d7d2b1d5b2589be37864521f43a5f4f5710b66888045de">
  
  
  

      <header>
      <h3>Latest Data Sets</h3>
    </header>
  
    
  
  <div class="item-list">
  
  <ul>

          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
      <a href="/help/foiadocsinvafoiahtm.html" hreflang="en">Information About Registered Investment Advisers and Exempt Reporting Advisers</a>
  </div></div><div class="views-field views-field-field-description-abstract"><div class="field-content">The Investment Adviser Information Reports&#039; data is collected from electronic submissions of Form ADV by investment adviser firms to the Investment Adviser Registration Depository (IARD) system. </div></div><div class="views-field views-field-field-date"><span class="views-label views-label-field-date">Updated</span><span class="field-content">    <time datetime="2018-05-01T14:20:00Z" class="datetime">May 2018</time>

</span></div></li>
          <li><div class="views-field views-field-field-display-title"><div class="field-content">
      	  
      <a href="/help/foiadocsbdfoiahtm.html" hreflang="en">Company Information About Active Broker-Dealers</a>
  </div></div><div class="views-field views-field-field-description-abstract"><div class="field-content">This text file contains the Central Index Key (CIK) numbers, company names, SEC reporting file numbers, and addresses (business addresses are provided when mailing addresses are not available) of active broker-dealers who are registered with the SEC.</div></div><div class="views-field views-field-field-date"><span class="views-label views-label-field-date">Updated</span><span class="field-content">    <time datetime="2018-05-01T14:00:00Z" class="datetime">May 2018</time>

</span></div></li>
    
  </ul>

</div>

  
    
  <div class="more-link"><a href="/data">More Data Sets</a></div>

    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
<div class="views-element-container block homepage_featured_content-we_provide_data">
  
    
      <div>
<div class="featured-content view view-homepage-featured-content view-id-homepage_featured_content view-display-id-we_provide_data js-view-dom-id-7a0d50743b8a9af2aaf0eaf522c88c201bd6ba65d82c9f2e4ed6cb260472004e">
  
  
  

      <header>
      
    </header>
  
    
  
  


        
        
  
  
  
    <div class="views-row promote view-row-count-1 view-row-first">
      <div class="views-field views-field-field-featured-graphic"><div class="field-content featured-graphic">  <a href="/structureddata">  <img class="image-style-featured-graphic" src="/files/styles/featured_graphic/public/2017-07/datadisclosure-spotlight.png?itok=z_m392wu" width="319" height="170" alt="Data and Disclosure" typeof="foaf:Image" />

</a>
</div></div><div class="views-field views-field-view-node"><h4 class="field-content featured-content-title"><a href="/structureddata" hreflang="en">Office of Structured Disclosure</a></h4></div><div class="views-field views-field-views-ifempty"><span class="field-content featured-content-teaser">The SEC&#039;s Office of Structured Disclosure is working to make financial reports more accessible and easy to use.</span></div>
    </div>

  

  
    
  
    
  
                <div id="table_paging">
        <span class="tgroup">
                </span>
        <center></center>
        <span class="tgroup1"> <span>
      </div>
      
</div>

</div>

  </div>
</div></div>
    </div>
  </section>

</div>

  </div>
</article>

  </div>

  </div>

      </div>
            
    </section>

    <section role="footer">
                <div>
    
<div id="block-globalfooterstayconnectedfooter" class="block stay-connected-footer">
  
    
        <div class="body"><p class="data-exempt" id="stay-connected-footer"><span>STAY CONNECTED</span><br class="new-line" />
<a href="/news/socialmedia.shtml"><span class="fa fa-lg fa-twitter"><span class="visually-hidden">1</span></span> <span class="hide-for-small">Twitter</span></a> <a href="/news/socialmedia.shtml"><span class="fa fa-lg fa-facebook"><span class="visually-hidden">2</span></span> <span class="hide-for-small">Facebook</span></a> <a href="/about/secrss.shtml"><span class="fa fa-lg fa-rss"><span class="visually-hidden">3</span></span><span class="hide-for-small">RSS</span></a> <a href="//www.youtube.com/user/SECViews/videos"><span class="fa fa-lg fa-youtube-play"><span class="visually-hidden">4</span></span><span class="hide-for-small">YouTube</span></a><br class="hide-for-medium-up" />
<a href="//www.flickr.com/photos/67083337@N02"><span class="fa fa-lg fa-flickr"><span class="visually-hidden">5</span></span> <span class="hide-for-small">Flickr</span></a> <a href="//www.linkedin.com/company/us-securities-and-exchange-commission?trk=mini-profile"> <span class="fa fa-lg fa-linkedin"><span class="visually-hidden">6</span></span><span class="hide-for-small">LinkedIn</span></a> <a href="//www.pinterest.com/secgov"><span class="fa fa-lg fa-pinterest-p"><span class="visually-hidden">7</span></span> <span class="hide-for-small">Pinterest</span></a> <a href="//public.govdelivery.com/accounts/USSEC/subscriber/new"><span class="fa fa-lg fa-envelope"><span class="visually-hidden">8</span></span> <span class="hide-for-small">Email Updates</span> </a></p>
</div>
  </div>
<nav role="navigation" aria-labelledby="block-secgov-footer-menu" id="block-secgov-footer">
            
  <h2 class="visually-hidden">Footer menu</h2>
  

        
              <ul>
              <li class="item-site-map">
        <a href="/sitemap.shtml" data-drupal-link-system-path="node/111831">Site Map</a>
              </li>
          <li class="item-accessibility">
        <a href="/disability/sec_access.htm" data-drupal-link-system-path="node/111766">Accessibility</a>
              </li>
          <li class="item-contracts">
        <a href="/about/offices/oacq.htm">Contracts</a>
              </li>
          <li class="item-privacy">
        <a href="/privacy.htm" data-drupal-link-system-path="node/111706">Privacy</a>
              </li>
          <li class="item-inspector-general">
        <a href="/oig" data-drupal-link-system-path="node/41456">Inspector General</a>
              </li>
          <li class="item-agency-financial-report">
        <a href="https://www.sec.gov/agency-financial-report">Agency Financial Report</a>
              </li>
          <li class="item-budget-&amp;-performance">
        <a href="/about/offices/ofm/ofm-documents.htm" data-drupal-link-system-path="node/111606">Budget &amp; Performance</a>
              </li>
          <li class="item-careers">
        <a href="/jobs.shtml">Careers</a>
              </li>
          <li class="item-contact">
        <a href="/contact-information/sec-directory" data-drupal-link-system-path="node/102846">Contact</a>
              </li>
          <li class="item-foia">
        <a href="/foia.shtml">FOIA</a>
              </li>
          <li class="item-no-fear-act-&amp;-eeo-data">
        <a href="/eeoinfo.shtml">No FEAR Act &amp; EEO Data</a>
              </li>
          <li class="item-whistleblower-protection">
        <a href="/eeoinfo/whistleblowers.htm" data-drupal-link-system-path="node/111891">Whistleblower Protection</a>
              </li>
          <li class="item-votes">
        <a href="/about/commission-votes.shtml" data-drupal-link-system-path="node/111231">Votes</a>
              </li>
          <li class="item-open-government">
        <a href="/open">Open Government</a>
              </li>
          <li class="item-plain-writing">
        <a href="/plainwriting.shtml" data-drupal-link-system-path="node/111701">Plain Writing</a>
              </li>
          <li class="item-links">
        <a href="/links.shtml">Links</a>
              </li>
          <li class="item-investor.gov">
        <a href="https://investor.gov/">Investor.gov</a>
              </li>
          <li class="item-usa.gov">
        <a href="https://www.usa.gov/">USA.gov</a>
              </li>
        </ul>
  


  </nav>

  </div>

          </section>
  </div>
</div>
</container>

<section role="off-canvas">

</section>
    

    <a href="#" class="back-to-top"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i>Return to Top</a>

    <div class="overlap">
  <!-- Subscribe link, RSS, Email -->
  <div id="addthis-icons-508" class="visibly-hidden">
    <div class="addthis-wrapper">
      <div class="appIconsDetail hide">
        <div class="addthis_toolbox addthis_default_style hide-for-small">
          <a class="addthis_button_print at300b" title="Print" href="#">
            <span class="fa fa-print"></span>
          </a>
          <a class="addthis_button_facebook at300b" title="Facebook" href="#">
            <span class="fa fa-facebook"></span>
          </a>
          <a class="addthis_button_twitter at300b" title="Tweet" href="#">
            <span class="fa fa-twitter"></span>
          </a>
          <a class="addthis_button_email at300b" target="_blank" title="Email" href="#">
            <span class="fa fa-envelope"></span>
          </a>
          <a class="addthis_button_compact at300m" href="#" title="Share">
            <span class="fa fa-plus"></span>
          </a>
        <div class="atclear"></div>
      </div>  
      <div class="addthis_toolbox hide">
        <a class="addthis_button_facebook at300b" title="Facebook" href="#">
          <span class="fa fa-facebook"></span>
        </a>
        <a class="addthis_button_twitter at300b" title="Tweet" href="#">
          <span class="fa fa-twitter"></span>
        </a>
        <a class="addthis_button_email at300b" target="_blank" title="Email" href="#">
          <span class="fa fa-envelope"></span>
        </a>
      </div>
      <div class="atclear"></div>
      </div>
    </div>
  </div>
  <script type="text/javascript" src="//s7.addthis.com/js/300/addthis_widget.js#async=1"></script>
</div>
    <script type="application/json" data-drupal-selector="drupal-settings-json">{"path":{"baseUrl":"\/","scriptPath":null,"pathPrefix":"","currentPath":"node\/2431","currentPathIsAdmin":false,"isFront":true,"currentLanguage":"en"},"pluralDelimiter":"\u0003","data":{"extlink":{"extTarget":false,"extClass":"0","extLabel":"","extImgClass":false,"extSubdomains":true,"extExclude":".*\\.gov|http:\/\/www.xbrl.org\/utr\/2013-05-17\/utr.xml|http:\/\/www.xbrl.org\/dtr\/type\/numeric-2009-12-16.xsd|http:\/\/www.xbrl.org\/dtr\/type\/nonNumeric-2009-12-16.xsd|https:\/\/secir.secure.force.com\/ombudsman\/OMMSForm","extInclude":"","extCssExclude":".data-exempt","extCssExplicit":"","extAlert":true,"extAlertText":"You are now leaving the SEC Website. The link you have selected is located on another server. Please click on the OK button below to proceed to the selected site. The SEC does not endorse this web site, its sponsor, or any of the policies, activities, products, or services offered on the site or by any advertiser on the site.","mailtoClass":"0","mailtoLabel":""}},"flexslider":{"optionsets":{"homepage_hero":{"animation":"fade","animationSpeed":600,"direction":"horizontal","slideshow":true,"easing":"swing","smoothHeight":false,"reverse":false,"slideshowSpeed":30000,"animationLoop":true,"randomize":true,"startAt":0,"itemWidth":0,"itemMargin":0,"minItems":0,"maxItems":0,"move":0,"directionNav":false,"controlNav":false,"thumbCaptions":false,"thumbCaptionsBoth":false,"keyboard":false,"multipleKeyboard":false,"mousewheel":false,"touch":true,"prevText":"Previous","nextText":"Next","namespace":"flex-","selector":".slides \u003E li","sync":"","asNavFor":"","initDelay":0,"useCSS":true,"video":false,"pausePlay":false,"pauseText":"Pause","playText":"Play","pauseOnAction":true,"pauseOnHover":false,"controlsContainer":"","manualControls":""}},"instances":{"flexslider-1":"homepage_hero"}},"user":{"uid":0,"permissionsHash":"34c5530e399151d56adc3e02e8041f71e09c3a4b8e95ff1c5442f13d79d0d783"}}</script>
<script src="/files/js/js_o-4iBG4GcmU4BG1AYF-HO54k6DuKxo3gzmBrkv7NkhA.js"></script>


  <script type="text/javascript">window.NREUM||(NREUM={});NREUM.info={"beacon":"bam.nr-data.net","licenseKey":"32edb8f179","applicationID":"55448943","transactionName":"ZQZSMBQEXxZZARJeXlxMcQcSDF4LFyYUQkFTD2wnCRdUOXUHCEJtdgZWBRMJRShdDBN7WFwIZBYDAHwEVgsWQl1TF18WFUgPAl0MA0VQRgZ5CgIASSRWBjVYQ0Y=","queueTime":0,"applicationTime":1574,"atts":"SUFRRlweTBg=","errorBeacon":"bam.nr-data.net","agent":""}</script></body>
  </html>
