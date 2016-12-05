var langs = ["en", "fr"];
var langCode = '';
var langJS = null;
console.log("On debug");

var translate = function (jsdata)
{	
	console.log("On translate");
	$("[tkey]").each (function (index)
	{
		var strTr = jsdata [$(this).attr ('tkey')];
	    $(this).html (strTr);
	});
}


langCode = navigator.language.substr (0, 2);

langs.forEach(function(element)
{	
	console.log("La langue de la page est : " + langCode);
	if(langCode == element)
	{
	$.getJSON("lang/"+langCode+".json", translate);
	}
	else
	{
	$.getJSON("lang/en.json", translate);
	}
},this);

