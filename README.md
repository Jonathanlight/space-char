Saisir tel : <input type="text" size="15" maxlength="10" onblur="return tel(this, '.')" />

<script>
function tel(element, separator) {
	var newvalue = "";
	for (var i = 0; i < element.value.length; i++) {
		if ((i > 0) && (i % 2 == 0)) {
			newvalue += separator;
		}
		newvalue += element.value.charAt(i);
	}
	element.value = newvalue;
	return true;
}
</script>
