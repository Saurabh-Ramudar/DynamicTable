<html>
	<head>
		<title>Create Table</title>
		<script type="text/javascript">
			function table(){
			var row=document.getElementById('row').value;
			var col=document.getElementById('col').value;
			document.write("No. of Rows: ",row,"<br>");
			document.write("No. of Columns: ",col);
			var a;
			a="<table border='1' height='400px' width='400px'>";
		
			for(i=0;i<row;i++){
			a+="<tr>";
			
			for(j=0;j<col;j++){
			a+="<th>Hi</th>";
			a+="<td></td>";}
			a+="</tr>";
			}
			a+="</table>";
			document.write(a);
			}
		</script>
	</head>
<body>
<form>
<label>Enter Number of rows:</label>
<input type="number" name="row" id="row" placeholder="Rows" required="">
<label>Enter Number of columns:</label>
<input type="number" name="col" id="col" placeholder="Columns" required="">
<input type="button" value="Create Table" onclick="table();">
</form>
</body>
</html>
