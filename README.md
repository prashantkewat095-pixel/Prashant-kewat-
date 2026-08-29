<!DOCTYPE html>
<html>
<head>
<title>Prashant Ki Website</title>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  text-align: center;
  background: lightblue;
  color: #222;
}

.card {
  max-width: 500px;
  margin: 30px auto;
  background: white;
  padding: 30px 20px;
  border-radius: 20px;
  box-shadow: 0 5px 15px #777;
}

img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  border: 5px solid lightblue;
}

h1 {
  font-size: 38px;
}

h2 {
  margin-top: 30px;
}

p {
  font-size: 20px;
}

button {
  font-size: 18px;
  padding: 14px 25px;
  margin: 8px;
  border: none;
  border-radius: 12px;
  background: lightblue;
  cursor: pointer;
}

button:active {
  transform: scale(0.95);
}

.section {
  margin-top: 25px;
}

#contact {
  display: none;
}

input, textarea {
  width: 90%;
  padding: 12px;
  margin: 8px;
  font-size: 17px;
  border: 1px solid #aaa;
  border-radius: 8px;
  box-sizing: border-box;
}

textarea {
  height: 100px;
}

.skill {
  display: inline-block;
  background: lightblue;
  padding: 10px 15px;
  margin: 5px;
  border-radius: 20px;
}
</style>
</head>

<body>

<div class="card">

<img src="https://www.w3schools.com/howto/img_avatar.png"
alt="Prashant">

<h1>👋 Prashant</h1>

<p>💻 Future Developer 🚀</p>

<button onclick="showAbout()">About Me</button>

<button onclick="sayHello()">Hello</button>

<button onclick="showContact()">Contact Me</button>


<div id="about" class="section">

<h2>👤 About Me</h2>

<p>My name is Prashant.</p>

<p>I am learning coding. 🚀</p>

<h2>🛠️ My Skills</h2>

<span class="skill">HTML</span>
<span class="skill">CSS</span>
<span class="skill">JavaScript</span>
<span class="skill">Python</span>

<h2>🚀 My Projects</h2>

<p>🌐 My First Website</p>
<p>💻 Learning JavaScript</p>
<p>🐍 Learning Python</p>

</div>


<div id="contact" class="section">

<h2>📞 Contact Me</h2>

<p>मुझे WhatsApp पर Message करें 👇</p>

<button onclick="whatsappMessage()">
💬 WhatsApp पर Message
</button>

</div>

</div>


<script>

function showAbout() {
  document.getElementById("about").style.display = "block";
}

function showContact() {
  document.getElementById("contact").style.display = "block";
  document.getElementById("contact").scrollIntoView();
}

function sayHello() {
  alert("Hello Prashant! 👋🎉");
}

function whatsappMessage() {
  window.open(
    "https://wa.me/919201429378?text=Hello%20Prashant!",
    "_blank"
  );
}

</script>

</body>
</html>
