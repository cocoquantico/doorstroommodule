# Blok 1 Algebra en rekenen
::: objective
In dit blok gaan we rekenen met breuken en letters. Als je straks in de 11e zit, ga je merken dat je dit bij veel onderwerpen moet toepassen.
:::
<p>Wat is 6 × 7?</p>
<input type="text" id="antwoord">
<button onclick="checkAntwoord()">Check</button>
<p id="feedback"></p>

<script>
  function checkAntwoord() {
    const val = document.getElementById("antwoord").value;
    const feedback = document.getElementById("feedback");
    if (val === "42") {
      feedback.innerText = "Goed gedaan!";
    } else {
      feedback.innerText = "Helaas, probeer het opnieuw.";
    }
  }
</script>
