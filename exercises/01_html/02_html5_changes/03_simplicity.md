# HTML5 syntax, forgiveness and brevity

## Exercises

Convert the following XHTML snippets to their HTML5 equivalents

### Doctype and HTML element

Assume the following document will not need to be XML-compliant.

```
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
	…
</html>
```

### Content-type and character-set

HTML5 uses a shorthand version of the Content-Type or Charset `meta` element. Replace this XHTML version with its HTML5 equivalent.

```
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
```

### Assumed defaults

HTML5 has a few default elements and attributes that make defining them obsolete. Whittle down the examples below.

```
<link rel="stylesheet" href="stylez.css" media="all" type="text/css" />
<script type="text/javascript" src="lolcakes.js" async="async"></script>
```

### Brevity

Strip this down to a bare-bones HTML5 document, using as few bytes as possible, but keep it valid.

```
<!DOCTYPE html>
<meta charset="utf-8">
<title>Succint HTML5 is Sweet-as?</title>
<link rel="stylesheet" href="/style.css">
<main role="main">
	<header role="banner">
		<h1>I <3 HTML5</h1>
	</header>
	<article>
		<p>HTML5 is great because:</p>
		<ul>
			<li>it’s more forgiving</li>
			<li>it’s more succint</li>
			<li>it has less syntactical requirements</li>
			<li>it ❤️'s UTF-8</li>
			<li>
				it comes packed with:
				<ul>
					<li>meaningful elements</li>
					<li>new input types</li>
					<li>extra webform attributes</li>
					<li>accessibility features such as ARIA and landmarks</li>
				</ul>
			<li>it allows for wrapping anchors</li>
			<li>and many more…</li>
		</ul>
	</article>
	<footer roler="contentino" id="copyright">
		<p>&copy; 2015 No-one. Ever.</p>
	</footer>
</main>
```