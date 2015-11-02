# XHTML syntax, well-formedness and validity

## Exercises

Make the following snippets XHTML1 (Strict) compliant.

### 1. Document setup and elements

XHTML has to comply to XML rules, such as how documents and elements are structured. Fix the following HTML by making it XHTML1 Strict-compliant.

```
<HTML>
	<TITLE>Hello world!
	<BODY>
		<P>Hello world!
	</BODY>
```

### 2. Element well-formedness

XHTML element tags need to follow strict patterns. Fix the following examples.

```
<IMG src="/lazy-dog.jpg">
<P>
	The <DEL>fantastic <INS>quick</INS></DEL> Mr. <INS>brown</INS></DEL> fox<BR>
	jumped over the lazy dog
```

### 3. Attributes

Attributes too need special care to be XML-compliant. Fix the following example.

```
<TEXTAREA name=message required>
```

### 4. Scripts

Some portions of an XML-compliant document might contain unwanted characters such as less-than (<) and ampersand (&) characters. How do we prevent those parts of the document from being parsed as XML?

```
<SCRIPT>
	for (var i=0; i<list.length; i++) {
		// do stuff & then beer.
	}
</SCRIPT>
```

