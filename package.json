const venom = require('venom-bot');

venom
  .create({
    session: 'bot-session',
    headless: true
  })
  .then((client) => start(client))
  .catch((erro) => {
    console.log(erro);
  });

function start(client) {
  client.onMessage((message) => {
    if (message.body.toLowerCase() === 'hola') {
      client.sendText(message.from, '¡Hola! Soy tu bot de prueba 🚀 en la nube');
    }
  });
}
