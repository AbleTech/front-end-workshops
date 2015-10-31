# HTML5 syntax, forgiveness and brevity

## Exercises

Convert the following XHTML snippets to their HTML5 equivalents

### Doctype and HTML element

Assume the following document will be served as `text/html`

```
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
	…
</html>
```

### Content-type and character-set

```
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
```

### Assumed defaults

```
<link rel="stylesheet" href="stylez.css" media="all" type="text/css" />
<script type="text/javascript" src="lolcakes.js"></script>
```

### Brevity

Strip this down to a bare-bones HTML5 document:

```
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
	<head>
		<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
		<title>Succint HTML5 is Sweet-as?</title>
		<link rel="stylesheet" type="text/css" href="/style.css" media="all" />
	</head>
	<body>
		<div id="wrapper">
			<div id="header">
				<h1>I &lt;3 HTML5</h1>
			</div>
			<div id="content">
				<p>HTML5 is great because:</p>
				<ul>
					<li>it&apos;s more forgiving</li>
					<li>it&apos;s more succint</li>
					<li>it has less syntactical requirements</li>
					<li>it &#2764;&#039;s UTF-8</li>
					<li>
						it comes packed with:
						<ul>
							<li>meaningful elements</li>
							<li>new input types</li>
							<li>extra webform attributes</li>
							<li>accessibility features such as ARIA and landmarks</li>
						</ul>
					</li>
					<li>it allows for wrapping anchors</li>
				</ul>
			</div>
			<div id="copyright">
				<p>&copy; 2015 No-one. Ever.</p>
			</div>
		</div>
	</body>
</html>
```