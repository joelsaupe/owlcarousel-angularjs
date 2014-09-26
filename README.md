**OwlCarousel-AngularJS**
AngularJS Wrapper for Owl Carousel
by: Joel Saupe, http://joelsaupe.com
date: 26 September 2014


**IMPLEMENTATION:**
Place directive in app.js
Include CSS and Javascript files
Make sure you have JQuery 1.7+ and AngularJS 1.2+

**HTML**

**PARAMETERS:**
Set carousel parameters with 'owl-[[parameter]]=""' In place of [[parameter]], use one of the 
JQuery parameters such as: items, pagination, singleItem, etc.
For a complete list of parameters see http://owlgraphic.com/owlcarousel/#customizing

Note: You must include 'owl-' before each parameter, this is to avoid collision with other 
plugins, such as Bootstrap 3.0.


**MULTIPLE CAROUSELS:**
Each carousel is uniquely identified by the element's id. If no id is assigned to the carousel
then 'owl-carousel' is used. This allows for controls on each carousel and the controls will
not affect any other carousel on the page



**CUSTOM CONTROLS:**
Apply the following classes to elements to assing them as control triggers.
 * '.[[carousel-id]]-next' = Scrolls Right
 * '.[[carousel-id]]-prev' = Scrolls Left
 * '.[[carousel-id]]-play' = Starts Autoplay
 * '.[[carousel-id]]-stop' = Stops Autoplay

Note: Replace [[carousel-id]] with the carousel's id, if no id is assigned then replace it with 'owl-carousel'


**EXAMPLE:**
	<div id="owlid" owlcarousel class="owl-carousel" owl-singleItem="true" owl-pagination="true">
	  <div class="owlid-items suggested-test" ng-repeat="item in items track by $index">
	     <h3>{{item}}</h3>
	  </div>
	</div>



**KNOWN BUGS**
Currently breaks when model is updated and a slide is added/removed. If you figure out how to fix it let me know!
