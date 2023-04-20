***
A principal novidade do HTTP/3 é que ele utiliza o protocolo de transporte QUIC (Quick UDP Internet Connections), em vez do TCP, que era usado nas versões anteriores do HTTP. Isso traz algumas melhorias significativas em relação ao HTTP/2, tais como:

1.  *Conexões mais rápidas*: o HTTP/3 utiliza o QUIC, que permite que as conexões sejam estabelecidas mais rapidamente e com menos atrasos, já que não é necessário estabelecer uma conexão separada para cada transferência de dados.
    
2.  *Menos perda de pacotes*: o QUIC inclui um mecanismo de retransmissão de pacotes perdidos, o que torna o protocolo menos suscetível a problemas de perda de pacotes na rede.
    
3.  *Melhor desempenho em conexões móveis*: o QUIC foi projetado para funcionar bem em redes móveis, onde a latência e a perda de pacotes podem ser mais frequentes.
    
4.  *Criptografia mais forte*: o HTTP/3 exige que todas as conexões sejam criptografadas, usando o protocolo de segurança TLS 1.3, o que aumenta a segurança da transmissão de dados.
    
5.  *Mais eficiente em termos de largura de banda*: o HTTP/3 é capaz de enviar múltiplos pedidos ao mesmo tempo, o que aumenta a eficiência da largura de banda.