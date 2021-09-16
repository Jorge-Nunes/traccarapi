*Whatsapp Gateway api Http Get or Traccar based on code Pedros Lopez Whatsapp.js* updated 16 Set 21

1.  Git Clone https://github.com/gyulamester/traccarapi
2.  npm install
3.  npm update
4.  node simple.js


**include in xml / Traccar**

<entry key='notificator.types'>web,sms</entry>
<entry key='notificator.sms.manager.class'>org.traccar.sms.HttpSmsClient</entry>
<entry key='sms.http.url'>http://localhost:8080/enviar?</entry>
<entry key='sms.http.template'>
{"destino": "{phone}","mensagem": "{message}", "token": "8s8d9s9fs991"}
</entry>
<entry key='status.timeout'>60</entry>


**send via http get for other purposes / Web**

http://localhost:8080/enviar?destino={phone}&mensagem={message}&token=8s8d9s9fs991


**Support for possible fixes**


*(Linux) error Sandbox / include in file ./node_modules/whatsapp-web.js/src/util/Constants.js* 
//fail load//


		exports.DefaultOptions = {
    puppeteer: {
        headless: true,
		args: ['--no-sandbox', '--disable-setuid-sandbox'],
        defaultViewport: null
    },

		
*Erro moduloraid ./node_modules/@pedroslopez/moduleraid/moduleraid.js* 
//UnhandledPromiseRejectionWarning: Error: Evaluation failed: TypeError: Cannot read properties of undefined (reading 'WidFactory')//

const moduleRaid = function () {
  moduleRaid.mID  = Math.random().toString(36).substring(7);
  moduleRaid.mObj = {};

  fillModuleArray = function() {
    webpackChunkwhatsapp_web_client.push([
      [moduleRaid.mID], {}, function(e) {
        Object.keys(e.m).forEach(function(mod) {
          moduleRaid.mObj[mod] = e(mod);
        })
      }
    ]);
  }
  
