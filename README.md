# Freshtohome<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>FreshEats - Food Delivery</title>
<style>
  body { margin:0; font-family:'Segoe UI', sans-serif; background:#fdf6f0; color:#333; }
  a { text-decoration:none; }
  header { background: linear-gradient(135deg, #ff6f00, #ff9100); padding:20px; color:white; text-align:center; box-shadow:0 4px 6px rgba(0,0,0,0.1); position: sticky; top:0; z-index:1000; }
  nav a { margin:0 15px; color:white; font-weight:bold; font-size:16px; }
  nav a:hover { text-decoration: underline; }
  .hero { background: url('https://images.unsplash.com/photo-1600891964599-f61ba0e24092') center/cover no-repeat; color:white; padding:100px 20px; text-align:center; position: relative; }
  .hero::after { content:""; position:absolute; top:0; left:0; width:100%; height:100%; background: rgba(0,0,0,0.4); }
  .hero h2, .hero p, .hero .btn { position: relative; z-index:1; }
  .hero h2 { font-size:3em; margin-bottom:15px; }
  .hero p { font-size:1.2em; margin-bottom:20px; }
  .btn { display:inline-block; padding:12px 25px; background:#ff5722; color:white; font-weight:bold; border-radius:50px; transition:0.3s; }
  .btn:hover { background:#e64a19; }
  .offers-container { width:90%; margin:30px auto; overflow:hidden; border-radius:15px; box-shadow:0 4px 12px rgba(0,0,0,0.15);}
  .offers { display:flex; animation: slide 12s infinite; }
  .offer { min-width:100%; background: linear-gradient(135deg,#ff8f00,#ff5722); color:white; text-align:center; padding:30px 20px; }
  .offer h3 { font-size:2em; margin-bottom:10px; }
  .offer p { font-size:1.2em; margin-bottom:15px; }
  .offer .btn { background:white; color:#ff5722; font-weight:bold; }
  @keyframes slide { 0%,33% { transform: translateX(0); } 34%,66% { transform: translateX(-100%); } 67%,100% { transform: translateX(-200%); } }
  .menu { padding:60px 20px; text-align:center; }
  .menu h2 { font-size:2.5em; margin-bottom:30px; color:#ff6f00; }
  .items { display:flex; justify-content:center; flex-wrap:wrap; gap:25px; }
  .item { background:white; border-radius:15px; width:250px; padding:15px; box-shadow:0 4px 12px rgba(0,0,0,0.1); transition:0.3s; }
  .item:hover { transform: translateY(-5px); box-shadow:0 6px 16px rgba(0,0,0,0.15);}
  .item img { width:100%; border-radius:15px; }
  .item h3 { margin-top:10px; color:#ff6f00; }
  .combos { padding:60px 20px; text-align:center; background:#fff3e0; }
  .combos h2 { font-size:2em; margin-bottom:30px; color:#ff6f00; }
  .combo-items { display:flex; justify-content:center; flex-wrap:wrap; gap:25px; }
  .combo { background:white; border-radius:15px; padding:15px; width:220px; box-shadow:0 4px 12px rgba(0,0,0,0.1); transition:0.3s; }
  .combo:hover { transform: translateY(-5px); box-shadow:0 6px 16px rgba(0,0,0,0.15); }
  .combo img { width:100%; border-radius:15px; }
  .combo h4 { margin-top:10px; color:#ff6f00; }
  .order-form { padding:60px 20px; background:#fff8e1; text-align:center; }
  .order-form h2 { font-size:2em; margin-bottom:20px; color:#ff6f00; }
  .order-form input, .order-form textarea { width:90%; padding:12px; margin:8px 0; border-radius:10px; border:1px solid #ccc; font-size:16px; }
  .order-form textarea { resize:none; height:70px; }
  .order-form button { background:#ff6f00; color:white; padding:14px 30px; border:none; border-radius:50px; font-size:18px; cursor:pointer; margin-top:10px; transition:0.3s; }
  .order-form button:hover { background:#e65c00; }
  table { width:90%; margin:20px auto; border-collapse:collapse; }
  th, td { border:1px solid #ffb74d; padding:10px; text-align:center; border-radius:5px; }
  th { background:#ffcc80; }
  footer { background:#ff6f00; color:white; padding:25px 10px; text-align:center; margin-top:40px; display:flex; flex-direction:column; gap:5px; align-items:center; }
  footer span { display:flex; align-items:center; gap:5px; }
  footer i { font-style:normal; }
  @media(max-width:768px){ .items,.combo-items { flex-direction:column; align-items:center; } .hero h2 { font-size:2.2em; } .hero p { font-size:1em; } }
</style>
</head>
<body>

<header>
  <h1>FreshEats</h1>
  <nav>
    <a href="#">Home</a>
    <a href="#">Menu</a>
    <a href="#order">Order</a>
    <a href="#">Contact</a>
  </nav>
</header>

<section class="hero">
  <h2>Delicious Food Delivered Fast 🍔</h2>
  <p>Order your favorite meals anytime, anywhere!</p>
  <a href="#order" class="btn">Order Now</a>
</section>

<div class="offers-container">
  <div class="offers">
    <div class="offer">
      <h3>🔥 20% OFF Today!</h3>
      <p>On all orders above ₹500</p>
      <a href="#order" class="btn">Order Now</a>
    </div>
    <div class="offer">
      <h3>🎉 Free Delivery!</h3>
      <p>On your first order</p>
      <a href="#order" class="btn">Order Now</a>
    </div>
    <div class="offer">
      <h3>🍔 Combo Deals</h3>
      <p>Buy 2 get 1 free on select items</p>
      <a href="#order" class="btn">Order Now</a>
    </div>
  </div>
</div>

<section class="menu">
  <h2>Popular Dishes</h2>
  <div class="items">
    <div class="item"><img src="https://images.unsplash.com/photo-1606756791042-8d8d2fdb2620" alt="Burger"><h3>Cheese Burger</h3></div>
    <div class="item"><img src="https://images.unsplash.com/photo-1604908177522-0400be2f1b8d" alt="Pizza"><h3>Veg Pizza</h3></div>
    <div class="item"><img src="https://images.unsplash.com/photo-1627308595181-1c52f9be3d9a" alt="Biryani"><h3>Hyderabadi Biryani</h3></div>
  </div>
</section>

<section class="combos">
  <h2>Popular Combos</h2>
  <div class="combo-items">
    <div class="combo"><img src="https://images.unsplash.com/photo-1617196031101-9b6ee022c05f" alt="Combo1"><h4>Burger + Coke</h4></div>
    <div class="combo"><img src="https://images.unsplash.com/photo-1594007658321-6cc3f8debc68" alt="Combo2"><h4>Pizza + Fries</h4></div>
    <div class="combo"><img src="https://images.unsplash.com/photo-1615486360477-f3f3cf7b1ed4" alt="Combo3"><h4>Biryani + Raita</h4></div>
  </div>
</section>

<section class="order-form" id="order">
  <h2>Place Your Order 🛒</h2>
  <form id="orderForm">
    <input type="text" id="name" placeholder="Your Name" required><br>
    <input type="text" id="phone" placeholder="Phone Number" required><br>
    <h3>Select Items</h3>
    <table>
      <tr><th>Food Item</th><th>Quantity</th></tr>
      <tr><td>Cheese Burger</td><td><input type="number" id="burgerQty" min="0" value="0"></td></tr>
      <tr><td>Veg Pizza</td><td><input type="number" id="pizzaQty" min="0" value="0"></td></tr>
      <tr><td>Hyderabadi Biryani</td><td><input type="number" id="biryaniQty" min="0" value="0"></td></tr>
    </table>
    <textarea id="otherItems" placeholder="Other Items (Coke, Fries, etc.)"></textarea><br>
    <input type="text" id="address" placeholder="Delivery Address" required><br>
    <button type="submit">Send Order via WhatsApp</button>
  </form>
</section>

<footer>
  <span>📞 +91 9876543210</span>
  <span>📧 support@fresheats.com</span>
  <span>💬 Order via WhatsApp</span>
</footer>

<script>
document.getElementById("orderForm").addEventListener("submit", function(e){
  e.preventDefault();
  let name = document.getElementById("name").value;
  let phone = document.getElementById("phone").value;
  let address = document.getElementById("address").value;
  let other = document.getElementById("otherItems").value;
  let burgerQty = document.getElementById("burgerQty").value;
  let pizzaQty = document.getElementById("pizzaQty").value;
  let biryaniQty = document.getElementById("biryaniQty").value;
  let order = "";
  if(burgerQty>0) order += `Cheese Burger x ${burgerQty}\n`;
  if(pizzaQty>0) order += `Veg Pizza x ${pizzaQty}\n`;
  if(biryaniQty>0) order += `Hyderabadi Biryani x ${biryaniQty}\n`;
  if(other.trim() !== "") order += `Other Items: ${other}\n`;
  if(order === "") { alert("Please select at least 1 item or enter other items."); return; }
  let message = `Hello, I want to order:\n\nName: ${name}\nPhone: ${phone}\nAddress: ${address}\n\nOrder Details:\n${order}`;
  let whatsappNumber = "918977143043";
  let url = `https://wa.me/${whatsappNumber}?text=${encodeURIComponent(message)}`;
  window.open(url,"_blank");
});
</script>

</body>
</html>
