+++
framed = true
+++

<div id="quote-box">damyge@damygectrl:~$ fortune<br> </div>

<script>
  document.addEventListener("DOMContentLoaded", function() {
    const quotes = fetch("quotes.md")
      .then(response => response.text())
      .then(data => data.split("%").map(quote => "damyge@damygectrl:~$ fortune<br>" + quote));

    const quoteBox = document.getElementById("quote-box");
    const nextSibling = quoteBox.nextElementSibling;
    
    if (nextSibling && nextSibling.tagName === "BLOCKQUOTE") {
      nextSibling.parentNode.removeChild(nextSibling);
    }

    quotes.then(quotesWithFortune => {
      quoteBox.innerHTML = quotesWithFortune[Math.floor(Math.random() * quotesWithFortune.length)];
    });
  });
</script>