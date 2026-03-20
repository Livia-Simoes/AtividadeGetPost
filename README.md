<div align="center">
<h1>SERVIDOR WEB</h1>
</div>

<br>

<div align="justify">
<hr><h2>MÉTODO POST 🖥️</h2>
<p><img width="1916" height="1030" alt="image" src="https://github.com/user-attachments/assets/9a94a30b-a5d6-4db6-a3d5-7738dd5c4fd5" />

 
</p>
</div>
<div align="justify">
<hr><h2>MÉTODO GET 🖥️</h2>
<p><img width="1910" height="1032" alt="Captura de tela 2026-03-20 103556" src="https://github.com/user-attachments/assets/a54dd951-fcc0-4a00-af0e-754ffb062e43" />


<hr><h2>Funcionamento do projeto:</h2>
<li>Método POST: o método POST foi o primeiro método testado, ele funciona enviando dados novos para o servidor processar, sendo utilizado mais para cadastro e login. 
  

tamanho = int(self.headers['Content-Length']):
esse código foi utilizado para descobrir o tamanho dos dados que o cliente (Postman) está enviando

dados = self.rfile.read(tamanho): 
esse código foi utilizado para ler o conteúdo enviado com base nesse tamanho

print("Dados recebidos!", dados.decode()):
esse código foi utilizado para mostrar no terminal do VS Code o que foi recebido


self.send_response(200) e self.end_headers() e self.wfile.write(b"POST recebido!"):
esse código foi utilizado para responder ao cliente que o dado foi aceito com sucesso


HTTPServer(("0.0.0.0", 8000), Servidor).serve_forever():
esse código foi utilizado para iniciar o servidor no endereço local e na porta 8000 </li>
<hr><li>Método GET: o Método GET foi o segundo método testado, ele funciona sem alterar nada, apenas lê os dados, sendo utilizado mais para ler sites de notícias, por exemplo.

self.send_response(200) e self.end_headers():
esse código foi utilizado para enviar o código 200 (OK), dizendo que a requisição deu certo

self.wfile.write(b"Servidor WEB Funcionando!"): 
esse código foi utilizado para escrever a resposta que o usuário vai ver no navegador ou Postman</li>
