---
layout: "v2_fluid/docs_base"
version: "nightly"
versionHref: "/docs/v2"
path: ""
category: api
id: "{{Refresher | slugify}}"
title: "Refresher"
header_sub_title: "Class in module "
doc: "Refresher"
docType: "class"
show_preview_device: true
preview_device_url: "/docs/v2/demos/refresher/"
angular_controller: APIDemoCtrl 
---









<h1 class="api-title">


Refresher






</h1>

<a class="improve-v2-docs" href='http://github.com/driftyco/ionic/edit/2.0/ionic/components/scroll/pull-to-refresh.ts#L6'>
Improve this doc
</a>






<!-- description -->

<p>Allows you to add pull-to-refresh to an Content component.
Place it as the first child of your Content or Scroll element.</p>
<p>When refreshing is complete, call <code>refresher.complete()</code> from your controller.</p>


<h3>Component</h3>
<h3>selector: <code>ion-refresher</code></h3>
<!-- @usage tag -->

<h3 style="margin-bottom: 7px">Usage</h3>


<pre><code class="lang-html">&lt;ion-content&gt;
  &lt;ion-refresher (starting)=&quot;doStarting()&quot;
                 (refresh)=&quot;doRefresh($event, refresher)&quot;
                 (pulling)=&quot;doPulling($event, amt)&quot;&gt;
  &lt;/ion-refresher&gt;

&lt;/ion-content&gt;
</code></pre>
<pre><code class="lang-ts">export class MyClass {
constructor(){}
  doRefresh(refresher) {
    console.log(&#39;Refreshing!&#39;, refresher);

    setTimeout(() =&gt; {
      console.log(&#39;Pull to refresh complete!&#39;, refresher);
      refresher.complete();
    })
  }

  doStarting() {
    console.log(&#39;Pull started!&#39;);
  }

  doPulling(amt) {
    console.log(&#39;You have pulled&#39;, amt);
  }
}
</code></pre>




<!-- @property tags -->

<h3>Attributes:</h3>
<table class="table" style="margin:0;">
<thead>
<tr>
<th>Attribute</th>
































<th>Type</th>


<th>Description</th>
</tr>
</thead>
<tbody>

<tr>
<td>
pullingIcon
</td>


<td>
string
</td>


<td>
the icon you want to display when you begin to pull down
</td>
</tr>

<tr>
<td>
pullingText
</td>


<td>
string
</td>


<td>
the text you want to display when you begin to pull down
</td>
</tr>

<tr>
<td>
refreshingIcon
</td>


<td>
string
</td>


<td>
the icon you want to display when performing a refresh
</td>
</tr>

<tr>
<td>
refreshingText
</td>


<td>
string
</td>


<td>
the text you want to display when performing a refresh
</td>
</tr>

<tr>
<td>
(refresh)
</td>


<td>
any
</td>


<td>
the methond on your class you want to perform when you refreshing
</td>
</tr>

<tr>
<td>
(starting)
</td>


<td>
any
</td>


<td>
the methond on your class you want to perform when you start pulling down
</td>
</tr>

<tr>
<td>
(pulling)
</td>


<td>
any
</td>


<td>
the methond on your class you want to perform when you are pulling down
</td>
</tr>

</tbody>
</table>


<!-- methods on the class -->

<h3>Methods</h3>

<div id="ele"></div>

<h3>
<code>ele()</code>
  

</h3>












<div id="isDragging"></div>

<h3>
<code>isDragging()</code>
  

</h3>












<div id="isOverscrolling"></div>

<h3>
<code>isOverscrolling()</code>
  

</h3>












<div id="dragOffset"></div>

<h3>
<code>dragOffset()</code>
  

</h3>












<div id="lastOverscroll"></div>

<h3>
<code>lastOverscroll()</code>
  

</h3>












<div id="ptrThreshold"></div>

<h3>
<code>ptrThreshold()</code>
  

</h3>












<div id="activated"></div>

<h3>
<code>activated()</code>
  

</h3>












<div id="scrollTime"></div>

<h3>
<code>scrollTime()</code>
  

</h3>












<div id="canOverscroll"></div>

<h3>
<code>canOverscroll()</code>
  

</h3>












<div id="pullingIcon"></div>

<h3>
<code>pullingIcon()</code>
  

</h3>












<div id="pullingText"></div>

<h3>
<code>pullingText()</code>
  

</h3>












<div id="refreshingIcon"></div>

<h3>
<code>refreshingIcon()</code>
  

</h3>












<div id="refreshingText"></div>

<h3>
<code>refreshingText()</code>
  

</h3>












<div id="spinner"></div>

<h3>
<code>spinner()</code>
  

</h3>












<div id="pulling"></div>

<h3>
<code>pulling()</code>
  

</h3>












<div id="refresh"></div>

<h3>
<code>refresh()</code>
  

</h3>












<div id="starting"></div>

<h3>
<code>starting()</code>
  

</h3>












<div id="content"></div>

<h3>
<code>content()</code>
  

</h3>










<!-- related link --><!-- end content block -->


<!-- end body block -->
