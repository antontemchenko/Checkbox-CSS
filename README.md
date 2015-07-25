# Checkbox-CSS
Changing style of checkbox with css3

# Demo
[Watch DEMO](http://anton.temchenko.com.ua/dev/css-checkbox.html)

# Code
`
<html>
	<head>
		<style>

			label {
			    position: relative;
			    font-size: 18px;
			    cursor: pointer;
			}

			input[type="checkbox"] {
			    -webkit-appearance: none;
			    -moz-appearance: none;
			    -ms-appearance: none;
			    -o-appearance: none;
			}

			input[type="checkbox"] + label:before {
			    content: '';
			    width: 15px;
			    height: 15px;
			    border-radius: 4px;
			    background: -webkit-linear-gradient(#D9E7F8, #81A9E0);
			    background: -moz-linear-gradient(#D9E7F8, #81A9E0);
			    background: -ms-linear-gradient(#D9E7F8, #81A9E0);
			    background: -o-linear-gradient(#D9E7F8, #81A9E0);
			    background: linear-gradient(#D9E7F8, #81A9E0);
			    border: 1px solid #888;
			    position: absolute;
			    left: -25px;
			    top: 1px;
			}

			input[type="checkbox"]:checked + label:before {
			  background: -webkit-linear-gradient(#E5FFE4, #3BEE3B);
			  background: -moz-linear-gradient(#E5FFE4, #3BEE3B);
			  background: -ms-linear-gradient(#E5FFE4, #3BEE3B);
			  background: -o-linear-gradient(#E5FFE4, #3BEE3B);
			  background: linear-gradient(#E5FFE4, #3BEE3B);
			}

			input[type="checkbox"] + label:after {
			    content: '';
			    display: none;
			    width: 4px;
			    height: 8px;
			    border: solid #3D6031;
			    border-width: 0 3px 3px 0;
			    -webkit-transform: rotate(45deg);
			    -moz-transform: rotate(45deg);
			    -ms-transform: rotate(45deg);
			    -o-transform: rotate(45deg);
			    transform: rotate(45deg);
			    position: absolute;
			    left: -20px;
			    top: 3px;
			}

			input[type="checkbox"]:checked + label:after {
			    display: block;
			}
		</style>
	</head>
	<body>
    <input id="1" type="checkbox"/>
    <label for="1">label 1</label>
	</body>
</html>`
