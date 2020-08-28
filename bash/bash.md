```jsx

//check for exit code of most recently executed 
echo $?

//do something here and we'll test for exit code
if [ "$?" = "0" ]; then
	echo "exit code was 0"
else
	echo "had another exit code" exit 111
fi

//test for file name and if it's readable
if [ -f $FILENAME ] && [ -r $FILENAME ] 
	then
		echo "exists and readable" 
fi

//elif and read values
//prompt for number
read NUMBER 
//go through if / elif
if [ "$NUMBER" -eq "1" ]; then 
	echo "got 1"
elif [ "$NUMBER" -eq "2" ]; then 
	echo "got 2"
elif [ "$NUMBER" -eq "3" ]; then 
	echo "got 3"
else
	echo "its another number"
fi

//send to /dev/null
echo "nobody will see this" >> /dev/null

//send stderr to /dev/null
<some action> 2>/dev/null

//focus on errors, stdout redirected to /dev/null, leaving only errors
<some action> 1>/dev/null
```