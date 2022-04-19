## Live Chat

É um chat que vai chamar o omnichannel.

Testando:
Para instalar Rocket.Chat Livechat no seu website, copie e cole este código acima da última tag **</ body>** em seu site.

```
<!-- Start of Rocket.Chat Livechat Script -->
	<script type="text/javascript">
	(function(w, d, s, u) {
		w.RocketChat = function(c) { w.RocketChat._.push(c) }; w.RocketChat._ = []; w.RocketChat.url = u;
		var h = d.getElementsByTagName(s)[0], j = d.createElement(s);
		j.async = true; j.src = 'http://159.203.108.195:3000/livechat/rocketchat-livechat.min.js?_=201903270000';
		h.parentNode.insertBefore(j, h);
	})(window, document, 'script', 'http://159.203.108.195:3000/livechat');
	</script>
```

__