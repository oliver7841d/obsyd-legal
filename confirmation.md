# Obsyd

<div id="ok">
<h2>Adresse confirmée ✓</h2>
<p><strong>Ton adresse email est bien confirmée, ton compte Obsyd est activé.</strong></p>
<p>Tu peux retourner dans l'app Obsyd et te connecter avec ton adresse email et ton mot de passe.</p>
<p>Tu peux fermer cette page.</p>
</div>

<div id="erreur" style="display:none">
<h2>Ce lien n'est plus valable</h2>
<p>Il a peut-être expiré ou a déjà été utilisé.</p>
<p>Si ton adresse est déjà confirmée, retourne simplement dans l'app Obsyd et connecte-toi.</p>
<p>Sinon, inscris-toi à nouveau depuis l'app avec la même adresse pour recevoir un nouveau lien, ou écris-nous à <a href="mailto:contact@obsyd.eu">contact@obsyd.eu</a>.</p>
</div>

<script>
  var infos = window.location.hash + window.location.search;
  if (infos.indexOf('error') !== -1) {
    document.getElementById('ok').style.display = 'none';
    document.getElementById('erreur').style.display = 'block';
  }
  if (window.location.hash) {
    history.replaceState(null, '', window.location.pathname);
  }
</script>
