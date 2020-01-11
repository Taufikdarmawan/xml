<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html b:version='2' class='v2' expr:dir='data:blog.languageDirection' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>
<head>
<meta charset='UTF-8'/>
<meta content='width=device-width, initial-scale=1.0' name='viewport'/>
</head>
<body>

<div id='body-wrapper'>
<div id='outer-wrapper'>

<div class='span-24'>

<div class='span-16'>
<div class='menu-primary-container'>
<ul class='menus menu-primary'>



</ul>
</div>
</div>
<div id='header-wrapper'>
<b:section class='header' id='headerbleft' maxwidgets='1' name='Header' showaddelement='no'>
  <b:widget id='Header1' locked='true' title='Seputan IT (Header)' type='Header' version='1'>
    <b:widget-settings>
      <b:widget-setting name='displayUrl'/>
      <b:widget-setting name='displayHeight'>0</b:widget-setting>
      <b:widget-setting name='sectionWidth'>932</b:widget-setting>
      <b:widget-setting name='useImage'>false</b:widget-setting>
      <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
      <b:widget-setting name='imagePlacement'>BEHIND</b:widget-setting>
      <b:widget-setting name='displayWidth'>0</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>

<b:if cond='data:useImage'>
<b:if cond='data:imagePlacement == &quot;REPLACE&quot;'>
<!--Show just the image, no text-->
<div id='header-inner'>
<a expr:href='data:blog.homepageUrl' style='display: block'>
  <img expr:alt='data:title' expr:height='data:height' expr:id='data:widget.instanceId + &quot;_headerimg&quot;' expr:src='data:sourceUrl' expr:width='data:width' style='display: block;padding-left:15px;padding-top:0px;'/>
</a>
</div>
<b:else/>
<!--
Show image as background to text. You can't really calculate the width
reliably in JS because margins are not taken into account by any of
clientWidth, offsetWidth or scrollWidth, so we don't force a minimum
width if the user is using shrink to fit.
This results in a margin-width's worth of pixels being cropped. If the
user is not using shrink to fit then we expand the header.
-->
<div expr:style='&quot;background-image: url(\&quot;&quot; + data:sourceUrl + &quot;\&quot;); &quot; + &quot;background-position: &quot; + data:backgroundPositionStyleStr + &quot;; &quot; + data:widthStyleStr + &quot;min-height: &quot; + data:height + &quot;px;&quot; + &quot;_height: &quot; + data:height + &quot;px;&quot; + &quot;background-repeat: no-repeat; &quot;' id='header-inner'>
<div class='titlewrapper' style='background: transparent'>
  <h1 class='title' style='background: transparent; border-width: 0px'>
    <b:include name='title'/>
  </h1>
</div>
<b:include name='description'/>
</div>
</b:if>
<b:else/>
<!--No header image -->
<div id='header-inner'>
<div class='titlewrapper'>
<h1 class='title'>
  <b:include name='title'/>
</h1>
</div>
<b:include name='description'/>
</div>
</b:if>
</b:includable>
    <b:includable id='description'>
<div class='descriptionwrapper'>
<p class='description'><span><data:description/></span></p>
</div>
</b:includable>
    <b:includable id='title'>
<a expr:href='data:blog.homepageUrl'><data:title/></a>
</b:includable>
  </b:widget>
</b:section>

<b:section class='headerbright' id='headerbright' maxwidgets='1' name='Ad Banner' showaddelement='yes'>
  <b:widget id='HTML7' locked='false' title='' type='HTML' version='1'>
    <b:includable id='main'>
  <b:if cond='data:title != &quot;&quot;'>
    <h2 class='title'><data:title/></h2>
  </b:if>
  <div class='widget-content'>
    <data:content/>
  </div>

  <b:include name='quickedit'/>
</b:includable>
  </b:widget>
</b:section>
<div style='clear:both;'/>
</div>
<div style='clear:both;'/>

<div style='clear:both;'/>

<div id='content-wrapper'>



<div id='crosscol-wrapper' style='text-align:center'>
<b:section class='crosscol' id='crosscol' showaddelement='yes'/>
</div>
<div id='main-wrapper'>
<b:section class='sitecontentarea' id='sitecontentarea' name='Blog' showaddelement='no'>
  <b:widget id='Blog1' locked='true' title='Blog Posts' type='Blog' version='1'>
    <b:widget-settings>
      <b:widget-setting name='showDateHeader'>true</b:widget-setting>
      <b:widget-setting name='style.textcolor'>#000000</b:widget-setting>
      <b:widget-setting name='showShareButtons'>true</b:widget-setting>
      <b:widget-setting name='authorLabel'>By</b:widget-setting>
      <b:widget-setting name='showCommentLink'>true</b:widget-setting>
      <b:widget-setting name='style.urlcolor'>#008000</b:widget-setting>
      <b:widget-setting name='showAuthor'>true</b:widget-setting>
      <b:widget-setting name='disableGooglePlusShare'>true</b:widget-setting>
      <b:widget-setting name='style.linkcolor'>#0000ff</b:widget-setting>
      <b:widget-setting name='style.unittype'>TextAndImage</b:widget-setting>
      <b:widget-setting name='style.bgcolor'>#ffffff</b:widget-setting>
      <b:widget-setting name='showAuthorProfile'>true</b:widget-setting>
      <b:widget-setting name='style.layout'>1x1</b:widget-setting>
      <b:widget-setting name='showLabels'>true</b:widget-setting>
      <b:widget-setting name='showLocation'>false</b:widget-setting>
      <b:widget-setting name='showTimestamp'>true</b:widget-setting>
      <b:widget-setting name='postsPerAd'>1</b:widget-setting>
      <b:widget-setting name='showBacklinks'>true</b:widget-setting>
      <b:widget-setting name='style.bordercolor'>#ffffff</b:widget-setting>
      <b:widget-setting name='showInlineAds'>false</b:widget-setting>
      <b:widget-setting name='showReactions'>true</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main' var='top'>
  <b:if cond='!data:mobile'>
    <!-- posts -->
    <div class='blog-posts hfeed'>

      <b:include data='top' name='status-message'/>

      <b:loop values='data:posts' var='post'>
        <b:if cond='data:post.isDateStart and not data:post.isFirstPost'>
          &lt;/div&gt;&lt;/div&gt;
        </b:if>
        <b:if cond='data:post.isDateStart'>
          &lt;div class=&quot;date-outer&quot;&gt;
        </b:if>
        <b:if cond='data:post.isDateStart'>
          &lt;div class=&quot;date-posts&quot;&gt;
        </b:if>
        <div class='post-outer'>
          <b:include data='post' name='post'/>
          <b:include cond='data:blog.pageType in {&quot;static_page&quot;,&quot;item&quot;}' data='post' name='comment_picker'/>
        </div>

        <!-- Ad -->
        <b:if cond='data:post.includeAd'>
          <div class='inline-ad'>
            <data:adCode/>
          </div>
        </b:if>
      </b:loop>
      <b:if cond='data:numPosts != 0'>
        &lt;/div&gt;&lt;/div&gt;
      </b:if>
    </div>

    <!-- navigation -->
    <b:if cond='data:blog.pageType != &quot;item&quot;'>
    <b:include name='nextprev'/>
    </b:if>

    <!-- feed links -->

  <b:else/>
    <b:include name='mobile-main'/>
  </b:if>

  <b:if cond='data:top.showPlusOne'>
    <data:top.googlePlusBootstrap/>
  </b:if>
  <div id='rsidebar-wrapper'>
<b:section class='sidebarpbt' id='sidebarleft' name='Right Sidebar' preferred='yes'>
  <b:widget id='Label1' locked='false' title='Categories' type='Label' version='1'>
    <b:widget-settings>
      <b:widget-setting name='sorting'>ALPHA</b:widget-setting>
      <b:widget-setting name='display'>LIST</b:widget-setting>
      <b:widget-setting name='selectedLabelsList'>Entertainment,Graphic Design,Motion Design,Print Design,Web Design</b:widget-setting>
      <b:widget-setting name='showType'>USER_SELECTED</b:widget-setting>
      <b:widget-setting name='showFreqNumbers'>true</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
  <b:if cond='data:title'>
    <h2><data:title/></h2>
  </b:if>
  <div expr:class='&quot;widget-content &quot; + data:display + &quot;-label-widget-content&quot;'>
    <b:if cond='data:display == &quot;list&quot;'>
      <ul>
      <b:loop values='data:labels' var='label'>
        <li>
          <b:if cond='data:blog.url == data:label.url'>
            <span expr:dir='data:blog.languageDirection'><data:label.name/></span>
          <b:else/>
            <a expr:dir='data:blog.languageDirection' expr:href='data:label.url'><data:label.name/></a>
          </b:if>
          <b:if cond='data:showFreqNumbers'>
            <span dir='ltr'>(<data:label.count/>)</span>
          </b:if>
        </li>
      </b:loop>
      </ul>
    <b:else/>
      <b:loop values='data:labels' var='label'>
        <span expr:class='&quot;label-size label-size-&quot; + data:label.cssSize'>
          <b:if cond='data:blog.url == data:label.url'>
            <span expr:dir='data:blog.languageDirection'><data:label.name/></span>
          <b:else/>
            <a expr:dir='data:blog.languageDirection' expr:href='data:label.url'><data:label.name/></a>
          </b:if>
          <b:if cond='data:showFreqNumbers'>
            <span class='label-count' dir='ltr'>(<data:label.count/>)</span>
          </b:if>
        </span>
      </b:loop>
    </b:if>
    <b:include name='quickedit'/>
  </div>
</b:includable>
  </b:widget>
  <b:widget id='HTML6' locked='false' title='Ordered List' type='HTML' version='1'>
    <b:widget-settings>
      <b:widget-setting name='content'>&lt;ol&gt;
&lt;li&gt;Lorem ipsum dolor sit amet, consectetuer adipiscing elit.&lt;/li&gt;
&lt;li&gt;Aliquam tincidunt mauris eu risus.&lt;/li&gt;
&lt;li&gt;Vestibulum auctor dapibus neque.&lt;/li&gt;
&lt;/ol&gt;</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
  <b:if cond='data:title != &quot;&quot;'>
    <h2 class='title'><data:title/></h2>
  </b:if>
  <div class='widget-content'>
    <data:content/>
  </div>

  <b:include name='quickedit'/>
</b:includable>
  </b:widget>
  <b:widget id='Text1' locked='false' title='Sample Text' type='Text' version='1'>
    <b:widget-settings>
      <b:widget-setting name='content'><![CDATA[Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation test link ullamco laboris nisi ut aliquip ex ea commodo consequat.<br />]]></b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
  <b:if cond='data:title != &quot;&quot;'>
    <h2 class='title'><data:title/></h2>
  </b:if>
  <div class='widget-content'>
    <data:content/>
  </div>

  <b:include name='quickedit'/>
</b:includable>
  </b:widget>
  <b:widget id='HTML4' locked='false' title='Definition List' type='HTML' version='1'>
    <b:widget-settings>
      <b:widget-setting name='content'>&lt;dl&gt;
&lt;dt&gt;Definition list&lt;/dt&gt;
&lt;dd&gt;Consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna 
aliqua.&lt;/dd&gt;
&lt;dt&gt;Lorem ipsum dolor sit amet&lt;/dt&gt;
&lt;dd&gt;Consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna 
aliqua.&lt;/dd&gt;
&lt;/dl&gt;</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
  <b:if cond='data:title != &quot;&quot;'>
    <h2 class='title'><data:title/></h2>
  </b:if>
  <div class='widget-content'>
    <data:content/>
  </div>

  <b:include name='quickedit'/>
</b:includable>
  </b:widget>
  <b:widget id='HTML3' locked='false' title='Support' type='HTML' version='1'>
    <b:widget-settings>
      <b:widget-setting name='content'><![CDATA[Need our help to <span style="font-weight:bold;">upload</span> or <span style="font-weight:bold;">customize</span> this blogger template? <a href="https://www.premiumbloggertemplates.com/contact/" target="_blank" rel="nofollow">Contact me</a> with details about the theme customization you need.]]></b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
  <b:if cond='data:title != &quot;&quot;'>
    <h2 class='title'><data:title/></h2>
  </b:if>
  <div class='widget-content'>
    <data:content/>
  </div>

  <b:include name='quickedit'/>
</b:includable>
  </b:widget>
  <b:widget id='PageList1' locked='false' title='Pages' type='PageList' version='1'>
    <b:widget-settings>
      <b:widget-setting name='pageListJson'>{}</b:widget-setting>
      <b:widget-setting name='homeTitle'>Home</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
  <b:if cond='data:title'><h2><data:title/></h2></b:if>
  <div class='widget-content'>
    <b:if cond='data:mobile'>
      <select expr:id='data:widget.instanceId + &quot;_select&quot;'>
        <b:loop values='data:links' var='link'>
          <b:if cond='data:link.isCurrentPage'>
            <option expr:value='data:link.href' selected='selected'><data:link.title/></option>
          <b:else/>
            <option expr:value='data:link.href'><data:link.title/></option>
          </b:if>
        </b:loop>
      </select>
      <span class='pagelist-arrow'>&#9660;</span>

    <b:else/>
      <ul>
        <b:loop values='data:links' var='link'>
          <b:if cond='data:link.isCurrentPage'>
            <li class='selected'><a expr:href='data:link.href'><data:link.title/></a></li>
          <b:else/>
            <li><a expr:href='data:link.href'><data:link.title/></a></li>
          </b:if>
        </b:loop>
      </ul>
    </b:if>
    <b:include name='quickedit'/>
  </div>
</b:includable>
  </b:widget>
</b:section>
</div>
</div> <!-- end content-wrapper -->

<div style='clear:both;'/>
<div id='footer-widgets-container'>
<div class='clearfix' id='footer-widgets'>

<div class='footer-widget-box'>
<ul class='widget-container'>
<li>
<b:section class='footersec' id='footersec1' name='Footer 1' showaddelement='yes'>
  <b:widget id='Feed1' locked='false' title='' type='Feed' version='1'>
    <b:widget-settings>
      <b:widget-setting name='feedUrl'>https://www.bloggertipandtrick.net/feed/</b:widget-setting>
      <b:widget-setting name='openLinksInNewWindow'>false</b:widget-setting>
      <b:widget-setting name='numItemsShow'>5</b:widget-setting>
      <b:widget-setting name='showItemDate'>false</b:widget-setting>
      <b:widget-setting name='showItemAuthor'>false</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
  <h2><data:title/></h2>
  <div class='widget-content' expr:id='data:widget.instanceId + &quot;_feedItemListDisplay&quot;'>
    <span style='filter: alpha(25); opacity: 0.25;'>
      <a expr:href='data:feedUrl'><data:loadingMsg/></a>
    </span>
  </div>
  <b:include name='quickedit'/>
</b:includable>
  </b:widget>
</b:section>
</li>
</ul>
</div>

<div class='footer-widget-box'>
<ul class='widget-container'>
<li>
<b:section class='footersec' id='footersec2' name='Footer 2' showaddelement='yes'>
  <b:widget id='Feed2' locked='false' title='' type='Feed' version='1'>
    <b:widget-settings>
      <b:widget-setting name='feedUrl'>https://www.premiumbloggertemplates.com/feed/</b:widget-setting>
      <b:widget-setting name='openLinksInNewWindow'>false</b:widget-setting>
      <b:widget-setting name='numItemsShow'>5</b:widget-setting>
      <b:widget-setting name='showItemDate'>false</b:widget-setting>
      <b:widget-setting name='showItemAuthor'>false</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
  <h2><data:title/></h2>
  <div class='widget-content' expr:id='data:widget.instanceId + &quot;_feedItemListDisplay&quot;'>
    <span style='filter: alpha(25); opacity: 0.25;'>
      <a expr:href='data:feedUrl'><data:loadingMsg/></a>
    </span>
  </div>
  <b:include name='quickedit'/>
</b:includable>
  </b:widget>
</b:section>
</li>
</ul>
</div>

<div class='footer-widget-box footer-widget-box-last'>
<ul class='widget-container'>
<li>
<b:section class='footersec' id='footersec3' name='Footer 3' showaddelement='yes'>
  <b:widget id='Text2' locked='false' title='Text Widget' type='Text' version='1'>
    <b:widget-settings>
      <b:widget-setting name='content'><![CDATA[Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation test link ullamco laboris nisi ut aliquip ex ea commodo consequat. <br /><br />Duis aute irure dolor in reprehenderit in voluptate another link velit esse cillum dolore eu fugiat nulla pariatur.<br />]]></b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
  <b:if cond='data:title != &quot;&quot;'>
    <h2 class='title'><data:title/></h2>
  </b:if>
  <div class='widget-content'>
    <data:content/>
  </div>

  <b:include name='quickedit'/>
</b:includable>
  </b:widget>
</b:section>
</li>
</ul>
</div>

</div>
</div>
<div style='clear:both;'/>

<div id='footer-container'>
<div id='footer'>   
<div id='copyrights'>
