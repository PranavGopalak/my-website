---
layout: page
title: "Calculator"
---

<h2>Simple Calculator</h2>
<p>Perform addition of two numbers.</p>

<form onsubmit="calculate(event)">
    <input type="number" id="num1" placeholder="First Number" required>
    <input type="number" id="num2" placeholder="Second Number" required>
    <button type="submit">Calculate</button>
</form>

<h3 id="result"></h3>

<script>
function calculate(event) {
    event.preventDefault();
    const num1 = parseFloat(document.getElementById('num1').value);
    const num2 = parseFloat(document.getElementById('num2').value);
    const result = num1 + num2;
    document.getElementById('result').textContent = `Result: ${result}`;
}
</script>
