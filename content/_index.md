+++
framed = true
+++

<div id="quote-box"> <br> </div>

<script>
    document.addEventListener("DOMContentLoaded", function() {
        const quotes = fetch("quotes.md")
        .then(response => response.text())
        .then(data => data.split("%").map(quote => "damyge@damygectrl:~$ fortune<br>" + quote));

    quotes.then(quotesWithFortune => {
        const quoteBox = document.getElementById("quote-box");
        quoteBox.innerHTML = quotesWithFortune[Math.floor(Math.random() * quotesWithFortune.length)];

    quoteBox.nextElementSibling?.remove();
  });
});
</script>