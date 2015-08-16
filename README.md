# DCM-HTML5-GSAP-inPage-Polite
This is to be used with DoubleClick Campaign Manager (DCM) and not DoubleClick Studio for a DoubleClick Studio version see: https://github.com/joemidi/DCRM-HTML5-GSAP-inPage-Polite

Without the Enabler.js file that DoubleClick Studio uses, the banner behaves much differently.

I've moved the polite loading script to the bottom of the HTML to stop it blocking.

I had to take the lazy loadScript from: http://www.nczonline.net/blog/2009/07/28/the-best-way-to-load-external-javascript/ as we were using the one built into Enabler.js previously.

Other things to note is the `<meta name="ad.size" content="width=300, height=250">` to describe the banner dimensions.

And declaring the *clickTags* in a script tag:
```
	<script type="text/javascript">
		var clickTag = "https://www.google.com";
		var clickTag1 = "https://www.github.com";
	</script>
```

_N.B. Not actually tested this build, and I'm not sure that DCM can use multiple clickTags_
