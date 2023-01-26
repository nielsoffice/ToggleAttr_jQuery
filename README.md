# ToggleAttr_jQuery
Hide and show attribute or toggle every time gets clicked! 

```HTML
<input id="_targt" type="checkbox">
<h1 id="testing"> Click me! </h1>

```

```JS

 jQuery(() => {
    
	let __target = jQuery('#testing'); // select elem you want to click
	let _targt 	 = '#_targt'; // elemt toggle attributes
	 
	  jQuery.fn.toggleAttr = function( _attr, _val ) {
		
		var attrRequest = jQuery(this).attr(_attr);
		
		if ( attrRequest ) 
		{ jQuery(this).removeAttr(_attr); } 
		else 
		{ jQuery(this).attr(_attr, _val); }
		  
		return this;
	  };
	 
	 jQuery( __target ).click(function() {
        jQuery( _targt ).toggleAttr("checked", "checked");
     })
 
 });
 
```
<br />
<hr />
<br />

<h5>Resources:</h5
<br /><a href="https://stackoverflow.com/questions/18665031/how-to-toggle-attr-in-jquery">Click Here</a>
<br /><a href="https://api.jquery.com/attr/">Docx Click Here</a>
<br /><a href="https://api.jquery.com/removeAttr/">Docx Click Here</a>

