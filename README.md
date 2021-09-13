Whatsapp Gateway api Http Get or Traccar based on code Pedros Lopez Whatsapp.js

npm install
npm update

--Traccar--

<entry key='notificator.types'>web,sms</entry>
<entry key='notificator.sms.manager.class'>org.traccar.sms.HttpSmsClient</entry>
<entry key='sms.http.url'>http://localhost:8080/enviar?</entry>
<entry key='sms.http.template'>
{"destino": "{phone}","mensagem": "{message}", "token": "8s8d9s9fs991"}
</entry>
<entry key='status.timeout'>60</entry>


--Web--

http://localhost:8080/enviar?destino={phone}&mensagem={message}&token=8s8d9s9fs991


Linux No Sandbox 
		args: ['--no-sandbox', '--disable-setuid-sandbox'],
		
Erro moduloraid

const moduleRaid = function () {
  moduleRaid.mID  = Math.random().toString(36).substring(7);
  moduleRaid.mObj = {};

  fillModuleArray = function() {
    (window.webpackChunkbuild || window.webpackChunkwhatsapp_web_client).push([
      [moduleRaid.mID], {}, function(e) {
        Object.keys(e.m).forEach(function(mod) {
          moduleRaid.mObj[mod] = e(mod);
        })
      }
    ]);
  }