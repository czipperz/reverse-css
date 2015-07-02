# Reverse-CSS

**Not built**

This takes valid CSS and makes it into code that groups by property instead of element. Here's an example:

    /* pre compilation */
    #title { color: red; background-color: #111; }
    a:link { color: white; background-color: black; }
	a:hover { color: red; background-color: black; }

    /* post compilation */
	#title, a:hover { color: red; }
	a:link, a:hover { background-color: black; }
	#title { background-color: #111; }
	a:link { color: white; }
