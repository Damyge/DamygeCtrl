+++
framed = true
+++

<div id="quote-box"> <br> </div>

<script>
  document.addEventListener("DOMContentLoaded", function() {
    const quotes = fetch("quotes.md")
      .then(response => response.text())
      .then(data => data.split("%").map(quote => "damyge@damygectrl:~$ fortune" + quote));

    quotes.then(quotesWithFortune => {
      document.getElementById("quote-box").innerHTML = quotesWithFortune[Math.floor(Math.random() * quotesWithFortune.length)];
    });
  });
</script>