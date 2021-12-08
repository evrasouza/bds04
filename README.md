<h1>Desafio</h1>
O professor Nelio Alves da Escola DevSuperior propôs como desafio para o final do capítulo 3 - Validação e segurança do Bootcamp Spring e React a tarefa abaixo.<br><br>

TAREFA: Validação e segurança<br><br>

Implemente as funcionalidades necessárias para que os testes do projeto abaixo passem: https://github.com/devsuperior/bds04<br><br>

Este é um sistema de eventos e cidades com uma relação N-1 entre eles:
Neste sistema, somente as rotas de leitura (GET) de eventos e cidades são públicas (não precisa de login). Usuários CLIENT podem também inserir (POST) novos eventos. Os demais acessos são permitidos apenas a usuários ADMIN.

<h3> Testes de Integração </h3> 
<h4> CityController </h4>
. Inserção de nova cidade deve retornar 401 quando usuário não estiver autenticado<br>
. Inserção de nova cidade deve retornar 403 quando usuário estiver autenticado não tiver permissão de inserir nova cidade<br>
. Inserção de nova cidade deve retornar 200 quando usuário administrador estiver autenticado<br>
. Inserção de nova cidade deve retornar 422 quando usuário administrador estiver autenticado e tentar inserir a cidade com o nome em branco<br>
. Busca deve retornar todas as cidades classificadas por nome<br><br>

<h4> EventController </h4>
. Inserção de nova cidade deve retornar 401 quando usuário não estiver autenticado<br>
. Inserção de nova cidade deve retornar 200 quando usuário estiver autenticado e enviar dados corretos<br>
. Inserção de nova cidade deve retornar 200 quando usuário Administrador estiver autenticado e enviar dados corretos<br>
. Inserção de novo Evento deve retornar 422 quando usuário administrador estiver autenticado e tentar inserir o Evento com o nome em branco<br>
. Inserção de novo Evento deve retornar 422 quando usuário administrador estiver autenticado e tentar inserir o Evento com data passada<br>
. Inserção de novo Evento deve retornar 422 quando usuário administrador estiver autenticado e tentar inserir o Evento com cidade nula<br
. Busca deve retornar todas os eventos<br><br>
