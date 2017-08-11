# Rython programming language
Python made right.

## Preamble
A programming language like any other instrument has its own pros and cons. 
You may say a language syntax is just secondary thing while the primary one is a good (useful, easy to understand, pragmatic, ...) semantics. But stop, syntax is our interface or gates to the language semantics. Bad interface anyway means bad interaction with codebases and bad readability. Supporting it fails. Even most great (read: optimal) architectures become obscured. 

There were many attempts to evolve C-like syntax to work with modern features in very large set of useful, time-proven languages like Java, PHP, etc. 
However somebody prefers different approaches. Leaving legacy and mature habits, trying something exotic and different. One of such tries is Python language. Poorly designed and hyped a lot it has still kinda potential to inherit. 
Rython project aims to drop all Python faults and keep best of two worlds: C-like syntactic space/indentation independency and concise expressions, consistent naming and other stuff.

## Why meaningful whitespaces are incorrect choice for programming language
To understand the point we should go back to the basics. Our main source code representation form is a text form. Moreover it is meant to be european language styled text form. We abstract from sentences and punctuation because our programming language is far from any natural one and there is no need to keep such properties. Anyway the core language features from the reader point of view are words, separated by spaces, and lines of text. Space widths may vary to justify line contents. Or to indicate indentation for better readability. Here we just note that whitespaces never used to indicate text structure. Line breaks - another virtual "character" also has no structural purpose. Speaking shortly, we can drop or insert line breaks between words, add more whitespaces or remove trailing ones but text meaning will not change after that. It is not applicable to words or punctuation, for example. Given reasons are enough to leave all syntaxes with meaningful whitespaces (and line breaks) and replace them with something more correct.

Here is an example what it could look like:

```python
if __module__ == "__main__":
    while true:
        try:
		num1 = int(raw_input(" Please give me a number: "));
		num2 = int(raw_input(" Please give me another number: "));;
	catch: print 'quiting'; break;;
        games = [
            ('+', lambda x,y: x + y),
            ('-', lambda x,y: x - y),
            ('*', lambda x,y: x * y),
            ('/', lambda x,y: float(x) / y),
        ];
        print " ***********************************";
        for game in games:
            op = func[0];
            result = game[1](num1, num2);
            print '%d %s %d = %s' % (num1, op, num2, result);;
        print " ***********************************";;
    
```
