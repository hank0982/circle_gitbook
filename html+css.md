# HTML+CSS

## What is HTML/CSS

Basically, most of the stuff you see on the internet are presented by what's called **HTML** and **CSS**. HTMLs can be in **.html** file form, created by javascript files, or a mixture of both, or in some other ways. CSSs can live inside .html files \(we call them **in-line CSS**, well, close enough\) or be included as a separate **.css** file.

Basically we can say: 

* HTMLs are the **actual content**
* CSSs are specifications of **how we display** the contents

## More into HTML

Anyway, let's look at a very very super-duper barebones .html file:

```markup
<!doctype html>

<html>

  <head>
    <title>Hello, world!</title>
  </head>
  
  <body>
    <p>You thought I'm going to put "Hello, world!" here but NO!</br>
      Wiiiiiiiiiii
    </p>
  </body>
  
</html>
```

So. Fret not, I'll go block by block.

First up,

```markup
<!doctype html>
```

This line declares that _this is an html file_. Not c, not c++, not js, not cat, not dog, and certainly not cat-dog.

Next, 

```markup
<html>
    // something something
</html>
```

{% hint style="info" %}
You may notice now that most stuff under line 1 comes in pairs. That's totally normal, as HTML is a MarkUP language.
{% endhint %}

**&lt;html&gt;&lt;/html&gt;** specifies that all the things within are _html contents_.

Most of the time, they're two main blocks in an html file:

```markup
<head></head>
```

which specifies _everything that's not directly contained in the display area_ of the webpage \(including which .css file to include, the title for each webpage, and the metadata for this webpage, etc.\), and

```markup
<body></body>
```

which specifies _everything that's being displayed._

So here we can see the title of the webpage is specified in the **&lt;head&gt;&lt;/head&gt;** block as

```markup
<title>Hello, world!</title>
```

And the content of this webpage is specified in the **&lt;body&gt;&lt;/body&gt;** block as 

```markup
<p>You thought I'm going to put "Hello, world!" here but NO!</br>
  Wiiiiiiiiiii
</p>
```

where **&lt;p&gt;&lt;/p&gt;** stands for **paragraph**, which is the standard way of putting text, and **&lt;/br&gt;** is the tag for **changing lines**. Think of &lt;/br&gt; as pressing the enter button when editing a word file.

So yeah. That's basically how an HTML file works.

{% hint style="success" %}
I'll salute you if you've read everything above word by word. Now, you should be able to find where all the basic elements are when given a random .html file. I hope.
{% endhint %}

## More into CSS

~~Just find something and try changing it a bit and see the results and you'll know what does what.~~

