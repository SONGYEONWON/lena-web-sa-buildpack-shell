# LENA WEB buildpack

레나 WEB proxy 서버를 Paas-ta / Cloud Foundry 에 적용하기위한 Buildpack 을 제공한다.

## How to
* 레나 WEB 서버 적용을 위해서는 proxy.conf 파일이 필요하다.
<pre><code>ProxyPassMatch ^/.*$ http://www.google.com</pre></code>
* cf push 시 빌드팩을 LENA WEB 으로 지정한다.
<pre><code>cf push -b https://github.com/lenalaborg/lena-web-buildpack1.0.git</pre></code>
* sample 디렉토리에 proxy.conf , manifest.yml 예제가 포함되어있다.
