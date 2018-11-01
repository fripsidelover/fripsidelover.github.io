<!--
%\VignetteEngine{knitr::knitr}
%\VignetteIndexEntry{Markdown example with knitr and googleVis}
-->






### 지역별 인구밀도 2013년도 - e나라지표

<br> 

* 자료출처:  e-나라지표 > 지표비교 > 부문별지표 > 총량지표 > 국토인구 > 지역현황 > 지역별 인구 및 인구밀도.
* e-나라지표 홈피 [링크](http://www.index.go.kr/potal/main/PotalMain.do). 

<br>

<!-- GeoChart generated in R 3.2.0 by googleVis 0.5.8 package -->
<!-- Sun May 31 07:59:18 2015 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataGeoChartID6886747ff0 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "KR-11",
16402 
],
[
 "KR-26",
4450 
],
[
 "KR-27",
2790 
],
[
 "KR-28",
2715 
],
[
 "KR-29",
3021 
],
[
 "KR-30",
2851 
],
[
 "KR-31",
1064 
],
[
 "KR-50",
259 
],
[
 "KR-41",
1193 
],
[
 "KR-42",
89 
],
[
 "KR-43",
210 
],
[
 "KR-44",
251 
],
[
 "KR-45",
223 
],
[
 "KR-46",
143 
],
[
 "KR-47",
139 
],
[
 "KR-48",
309 
],
[
 "KR-49",
308 
] 
];
data.addColumn('string','region_code');
data.addColumn('number','X2013.pop_density');
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataTableID68840c67100 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 9926,
16402 
],
[
 3426,
4450 
],
[
 2465,
2790 
],
[
 2826,
2715 
],
[
 1514,
3021 
],
[
 1540,
2851 
],
[
 1129,
1064 
],
[
 120,
259 
],
[
 12137,
1193 
],
[
 1500,
89 
],
[
 1552,
210 
],
[
 2060,
251 
],
[
 1798,
223 
],
[
 1761,
143 
],
[
 2641,
139 
],
[
 3255,
309 
],
[
 570,
308 
],
[
 24890,
2106 
] 
];
data.addColumn('number','2013 pop');
data.addColumn('number','2013 pop_density');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartGeoChartID6886747ff0() {
var data = gvisDataGeoChartID6886747ff0();
var options = {};
options["width"] =    700;
options["height"] =    400;
options["region"] = "KR";
options["displayMode"] = "regions";
options["resolution"] = "provinces";

    var chart = new google.visualization.GeoChart(
    document.getElementById('GeoChartID6886747ff0')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartTableID68840c67100() {
var data = gvisDataTableID68840c67100();
var options = {};
options["allowHtml"] = true;
options["height"] =    300;
options["width"] =    200;

    var chart = new google.visualization.Table(
    document.getElementById('TableID68840c67100')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "geochart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartGeoChartID6886747ff0);
})();
function displayChartGeoChartID6886747ff0() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}


// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "table";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartTableID68840c67100);
})();
function displayChartTableID68840c67100() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartGeoChartID6886747ff0"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID68840c67100"></script>
 
<table border="0">
<tr>
<td>

<!-- divChart -->
  
<div id="GeoChartID6886747ff0" 
  style="width: 700; height: 400;">
</div>

</td>
<td>

<!-- divChart -->
  
<div id="TableID68840c67100" 
  style="width: 200; height: 300;">
</div>

</td>
</tr>
</table>
