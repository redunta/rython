# righton
Python made right.

if __ima__ == "__glav__":
    poka istina:
        popit:
			num1 = celoe(raw_input(" Please give me a number: "));
			num2 = celoe(raw_input(" Please give me another number: "));;
		lovit: print 'quiting'; slom;;
        igri = [
            ('+', lambda x,y: x + y),
            ('-', lambda x,y: x - y),
            ('*', lambda x,y: x * y),
            ('/', lambda x,y: float(x) / y),
        ];
        pechat " ***********************************";
        dla igra v igri:
            op = func[0];
            result = igra[1](num1, num2);
            pechat '%d %s %d = %s' % (num1, op, num2, result);;
        pechat " ***********************************";;
    
   
		// print->pechat, catch->lovit, throw->kinut, finally->nakon, try->popit, break->slom
