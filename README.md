# Rython programming language
Python made right.

A programming language like any other instrument has its own pros and cons. 
You may say a language syntax is just secondary thing while the primary one is a good (useful, easy to understand, pragmatic, ...) semantics. But stop, syntax is our interface or gates to the language semantics. Bad interface anyway means bad interaction with codebases and bad readability. Supporting it fails. Even most great (read: optimal) architectures become obscured. 

There were many attempts to evolve C-like syntax to work with modern features in very large set of useful, time-proven languages like Java, PHP, etc. 
However somebody prefers different approaches. Leaving legacy and mature habits, trying something exotic and different. One of such tries is Python language. Poorly designed and hyped a lot it has still kinda potential to inherit. 
Rython project aims to drop all Python faults and keep best of two worlds: C-like syntactic space/indentation independency and concise expressions, consistent naming and other stuff.

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
