# kashaf
<html>
<head>
<title>Count number of words in a string</title>
</head>
<body>
<textarea id="InputText" cols="30" rows="4">enter string.</textarea>
<br>
<input type="button" name="Convert" value="No. of Words" onClick="count_words();">
<input id = "noofwords" type="text" value="" size="6"> 
<script>function count_words()
{
str1= document.getElementById("InputText").value;
str1 = str1.replace(/(^\s*)|(\s*$)/gi,"");  
str1 = str1.replace(/[ ]{2,}/gi," ");
str1 = str1.replace(/\n /,"\n");
document.getElementById("noofwords").value = str1.split(' ').length;
}
</script>
</body>
</html>
