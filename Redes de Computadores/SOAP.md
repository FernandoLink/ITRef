
##### *SOAP - Service Object Access Protocol*
É uma protocolo de mensagens baseado em XML para trocar informações entre computadores.
***

Uma mensagem SOAP é um documento XML que contém os seguintes elementos:

* **Envelope** - Define o início e o fim da mensagem. É um elemento obrigatório.
* **Header** - Contém quaisquer atributos opcionais da mensagem utilizados no processamento da mensagem. É um elemento opcional.
* **Body** - Contém os dados XML que compõem a mensagem a ser enviada. É um elemento obrigatório.
* **Fault** - Um elemento opcional de falha que fornece informação sobre erros que ocorrem no processamento da mensagem.


Estrutura Geral de uma mensagem SOAP:

```
<?xml version = "1.0"?>
<SOAP-ENV:Envelope xmlns:SOAP-ENV = "http://www.w3.org/2001/12/soap-envelope" 
   SOAP-ENV:encodingStyle = "http://www.w3.org/2001/12/soap-encoding">

   <SOAP-ENV:Header>
      ...
      ...
   </SOAP-ENV:Header>
   <SOAP-ENV:Body>
      ...
      ...
      <SOAP-ENV:Fault>
         ...
         ...
      </SOAP-ENV:Fault>
      ...
   </SOAP-ENV:Body>
</SOAP_ENV:Envelope>
```


|Tipo			|	Conteúdo                       |
|----|----------|
|string				|	Confirm this is electric.                  |
|boolean			|		true, false, 1, 0.                     |
|float				|	-INF, -1E4, -0, 0, 12.78E-2, 12, INF, NaN. |
|double				|	-INF, -1E4, -0, 0, 12.78E-2, 12, INF, NaN. |
|decimal			|	-1.23, 0, 123.4, 1000.00.                  |
|binary				|	100010                                     |
|integer			|			-126789, -1, 0, 1, 126789.         |
|nonPositiveInteger	|		-126789, -1, 0.                        |
|negativeInteger	|		-126789, -1.                           |
|long				|	-1, 12678967543233                         |
|int				|	-1, 126789675                              |
|short				|			-1, 12678                          |
|byte				|		-1, 126                                |
|nonNegativeInteger	|0, 1, 126789                                  |
|unsignedLong		|		0, 12678967543233                      |
|unsignedInt		|			0, 1267896754                      |
|unsignedShort		|		0, 12678                               |
|unsignedByte		|			0, 126                             |
|positiveInteger	|				1, 126789.                     |
|date				|		1999-05-31, ---05.                     |
|time				|			13:20:00.000, 13:20:00.000-05:00   |


##### SITE
***
[W3-SOAP](https://www.w3.org/TR/soap/)



