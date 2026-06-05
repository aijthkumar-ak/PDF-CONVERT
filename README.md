<!DOCTYPE html>
<html>
<head>
    <title>Daily Expense Tracker</title>
</head>
<body>
<h2>Daily Expense Tracker</h2>
<input type="date" id="date">
<input type="text" id="expenseName" placeholder="Expense Name">
<input type="number" id="amount" placeholder="Amount">
<button onclick="addExpense()">Add Expense</button>
<h3>Expenses List</h3>
 <ul id="expenseList"></ul>
<h3>Total Expenses: ₹<span id="total">0</span></h3>
<script>
let total = 0;
function addExpense() {
    let date = document.getElementById("date").value;
    let name = document.getElementById("expenseName").value;
    let amount = Number(document.getElementById("amount").value);
    if (!date || !name || amount <= 0) {
        alert("Please fill all fields");
        return;
    }
    let li = document.createElement("li");
    li.textContent = `${date} - ${name} : ₹${amount}`;    document.getElementById("expenseList").appendChild(li);
    total += amount;    document.getElementById("total").textContent = total;   document.getElementById("expenseName").value = "";    document.getElementById("amount").value = "";
}
</script>

</body>
</html>
