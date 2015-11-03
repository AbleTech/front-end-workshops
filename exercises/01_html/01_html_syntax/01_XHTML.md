# XHTML syntax, well-formedness and validity

## Exercises

Make the following snippets XHTML1 (Strict) compliant.

### 1. Document setup and elements

XHTML has to comply to XML rules, such as how documents and elements are structured. Fix the following HTML by making it XHTML1 Strict-compliant.

```
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
        "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
  <head>
    <title>Hello world!</title>
  </head>
	<body>
		<p>Hello world!</p>
	</body>
</html>
```

### 2. Element well-formedness

XHTML element tags need to follow strict casing, nesting and closing patterns. Fix the following snippets...

```
<img src="/lazy-dog.jpg" alt="image"/>
<p>
	The <del>fantastic</del> <ins>quick</ins> <del>Mr.</del> <ins>brown</ins> fox<br />
	jumped over the lazy dog
</p>
```

### 3. Attributes

Attributes too need special care to be XML-compliant. Fix the following example. (Bonus points for writing the `textarea` element correctly)

```
<textarea name="message" required="required"></textarea>
```

### 4. Scripts and style blocks

Some portions of an XML-compliant document might contain unwanted characters such as less-than (<) and ampersand (&) characters. How do we prevent those parts of the document from being parsed as XML?

```
<script type="text/javascript">
//<![CDATA[
	for (var i=0; i<list.length; i++) {
		// do stuff & then beer.
	}
//]]>
</script>
```

### 5. Character entities

Replace the following characters with their associated entities

```
©
™
&
💩
```