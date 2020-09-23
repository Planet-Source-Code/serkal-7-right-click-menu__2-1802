<div align="center">

## RIGHT CLICK MENU


</div>

### Description

Have you ever wanted a navigation menu instead of Internet Exporer's right click menu. Well now you can. This script will have a menu (which you can adjust the height, amount of links, font and color in the source. BUT THIS ONLY WORKS WITH MICROSOFT INTERNET EXPLORER 5.0
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[SeRkaL\_7](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/serkal-7.md)
**Level**          |Advanced
**User Rating**    |4.3 (17 globes from 4 users)
**Compatibility**  |
**Category**       |[Controls/ Forms/ Graphics/ Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/controls-forms-graphics-menus__2-59.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/serkal-7-right-click-menu__2-1802/archive/master.zip)





### Source Code

```
<html>
<head>
<title>Right Click Menu</title>
<style>
<!--
/*
This Script only works with Internet Explorer 5.0
*/
#ie5menu{
position:absolute;
width:150px;
border:2px solid blue;
background-color:navy;
font-family:Tahoma;
line-height:20px;
cursor:default;
visibility:hidden;
}
.menuitems{
padding-left:15px;
padding-right:15px;
}
-->
</style>
<!--[if IE]>
<div id="ie5menu" onMouseover="highlightie5()" onMouseout="lowlightie5()" onClick="jumptoie5()">
<div class="menuitems" url="http://your-site.com">LINK 1</div>
<div class="menuitems" url="http://your-site.com">LINK 2</div>
<div class="menuitems" url="http://your-site.com">LINK 3</div>
<div class="menuitems" url="http://your-site.com">LINK 4</div>
<hr>
<div class="menuitems" url="http://your-site.com">LINK 5</div>
<div class="menuitems" url="http://your-site.com">LINK 6</div>
<div class="menuitems" url="http://your-site.com">LINK 7</div>
<div class="menuitems" url="http://your-site.com">LINK 8</div>
<hr>
<div class="menuitems" url="mailto:yourname@domain.com">Email Me</div>
</div>
<![endif]-->
</head>
<BODY bgcolor="#000000 fontcolor="#FFFFFF" bgproperties="fixed">
<script language="JavaScript1.2">
var display_url=1
function showmenuie5(){
ie5menu.style.left=document.body.scrollLeft+event.clientX
ie5menu.style.top=document.body.scrollTop+event.clientY
ie5menu.style.visibility="visible"
return false
}
function hidemenuie5(){
ie5menu.style.visibility="hidden"
}
function highlightie5(){
if (event.srcElement.className=="menuitems"){
event.srcElement.style.backgroundColor="highlight"
event.srcElement.style.color="white"
if (display_url==1)
window.status=event.srcElement.url
}
}
function lowlightie5(){
if (event.srcElement.className=="menuitems"){
event.srcElement.style.backgroundColor=""
event.srcElement.style.color="black"
window.status=''
}
}
function jumptoie5(){
if (event.srcElement.className=="menuitems")
window.location=event.srcElement.url
}</script><script
language="JavaScript1.2">
document.oncontextmenu=showmenuie5
if (document.all&&window.print)
document.body.onclick=hidemenuie5</script>
Right click to see the menu<br>
</body>
</html>
```

