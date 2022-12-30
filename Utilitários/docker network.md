***
A rede **bridge** é a rede padrão criada pelo Docker quando ele é instalado. Ela permite que os contêineres se comuniquem entre si e com o host, assim como acessar a Internet, se necessário.

Quando você cria um contêiner no Docker, ele é adicionado automaticamente à rede bridge. Isso significa que, por padrão, todos os contêineres criados no Docker são capazes de se comunicar uns com os outros e com o host usando a rede bridge.

Você pode criar suas próprias redes no Docker e conectar os contêineres a elas, mas a rede bridge é criada automaticamente e é a opção padrão para conectar contêineres entre si e com o host.

***
A rede **host** é uma opção de rede no Docker que permite que o contêiner use a rede do host em vez de uma rede isolada criada pelo Docker. Isso significa que o contêiner compartilha o endereço IP e a stack de rede do host, o que o torna capaz de se comunicar com outros contêineres e com o host da mesma forma que um processo no host poderia.

Usar a rede host pode ser útil em alguns casos, como quando você precisa que o contêiner tenha acesso a recursos da rede do host, como serviços de rede, ou quando precisa garantir que o contêiner tenha um endereço IP acessível pelo host.

***
A rede **none** não vai ter nenhuma interface de rede, ele ficou isolado.
