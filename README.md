# Classe CURL para restful

### GET
```php
$curl = new Curl;

//Envio simples
$curl->get("http://localhost/pagina"); 

//Envio com parametros
$curl->get("http://localhost/pagina?nome=Carlos&id=3"); 
```

### POST
```php
$curl = new Curl;

//Envio simples
$curl->post("http://localhost/pagina"); 

//Envio com parametros
$dados = array('nome' => 'Carlos', 'id' => 3);
$curl->post("http://localhost/pagina", $dados); 
```

#### POST com envio de arquivo
```php
$curl = new Curl;

//Envio de parametros e arquivo (Sempre usar o @ antes do local do arquivo)
$dados = array('titulo' => 'arquivo1', 'arquivo' => '@'.basename('arquivo.txt'));
$curl->post("http://localhost/pagina", $dados); 
```

### PUT
```php
$curl = new Curl;

//Envio simples
$curl->put("http://localhost/pagina"); 

//Envio com parametros
$dados = array('nome' => 'Carlos', 'id' => 3);
$curl->put("http://localhost/pagina", $dados); 
```

### DELETE
```php
$curl = new Curl;

//Envio simples
$curl->delete("http://localhost/pagina"); 

//Envio com parametros
$dados = array('nome' => 'Carlos', 'id' => 3);
$curl->delete("http://localhost/pagina", $dados); 
```


----
**Author** Carlos W. Gama

Livre para usar, modificar e destribuir como desejar