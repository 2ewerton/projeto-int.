 *<h1> Fenix Tecnologia <h1>*

 *<h3>- Dieta: </h3>* Este módulo vai contar com duas interfaces diferentes, onde a interface do profissional de nutrição irá alimentar uma lista com os tópicos de alimento, horário e quantidade.
 Na interface do paciente, irá aparecer todas as informações que foram passadas pela nutricionista ao mesmo, em contrapartida o paciente deverá alimentar a mesma lista, dizendo o que ele comeu em cada refeição, as quantidades e os horários. 

 *<h3>- Alarme: </h3>* Este módulo irá contar com duas interfaces diferentes, onde a interface do profissional de nutrição irá acrescentar horário para o paciente ingerir alimentos e água.
 Na interface do paciente, irá aparecer todas as informações que foram passadas pela nutricionista ao mesmo, em contrapartida o paciênte deverá alimentar a mesma lista,confirmando os horários ou alterando conforme sua disponibilidade.
 
 *<h3>- Acompanhamento de Peso: </h3>* Módulo que ajuda o usuário a compreender seus hábitos alimentares registrando as calorias consumidas. Vai possuir monitoramento de gordura, proteínas, carboidratos e colesterol.

 *<h3>- Gráfico de Evolução: </h3>* Gráfico que ficará disponível a ambos usuários que será alimentado pelas informações que o paciente inserir no aplicativo, como taxas de colesterol e glicose, calorias ingeridas e peso  atual.

 *<h3>- Atividade Física: </h3>* Neste módulo será opcional o uso do mesmo, se o profissional de nutrição julgar necessário a realização de exercícios físicos o mesmo poderá recomendar ao seu paciente, nele terá exercícios padrões e a opção de listar um outro exercício. Na interface do paciente ele poderá conferir quais exercícios foram recomendados para ele e também um exemplo de como o exercício é executado.

 *<h3>- Agendamento de consultas: </h3>* Módulo onde o paciente pode solicitar ao seu nutricionista uma consulta não prevista.

<h2> Documento de definição de requisitos </h2>

*<h3>Requisitos Funcionais</h3>*

Requisitos Func. | Descrição | Prioridade |Depende de|
|:-----------------:|:-----------:|:------------:|:----------:|
 RF 01 |Efetuar Cadastro (Nutricionista / Paciente)| Alta|--|
 RF 02 |Efetuar Login / LogOff ( Nutricionista / Paciente )| Média|RF 01|
 RF 03 |Acessar Menu com todas as funcionalidades do app ( Nutricionista )| Média|RF 01 / RF 02|
 RF 04 |Poder criar dietas|Alta|--|
 RF 05 |Sugerir Horários ( Alimentação, Atividade Física, Sono e etc..)| Média | RF 04 |
 RF 06 |Sugestões do Nutricionista|Baixa|--|
 RF 07 |Criação de relatórios|Alta|--|
 RF 08 |Sugestão de atividades físicas|Média|--|
 RF 09 |Agendamento de consultas|Média|--|
 RF 10 |Acessar Menu do paciente|Média|RF 03|
 RF 11 |Poder cadastrar, atualizar e excluir clientes/pacientes|Média|RF 10|
 RF 12 |Geração de relatórios|Médio|RF 10|
 RF 13 |Acompanhamento de resultados|Alto|RF 12|
 RF 14 |Primeiro acesso Paciente ( Questionário: idade , peso, altura, objetivo, sexo e exames ) | Alto | RF 02 |
 RF 15 |Atualização de cadastro ( Paciente)| Médio | RF 01 / RF 02 |
 RF 16 |Acesso ao Menu ( Paciente ) | Alto | RF 02 |
 RF 17 |Visualizar dietas e sugestão de horários estipulados pelo nutricionista (Paciente)| Alto | RF 04 / RF 05 |
 RF 18 |Questionários de acompanhamento ( Paciente ) | Médio | -- |
 RF 19 |Acompanhamento de objetivos ( Paciente ) | Médio | RF 18 | 
 RF 20 |Visualizar gráficos de evolução ( Paciente ) | Médio | RF 18 / RF 19 |
 RF 21 |Visualizar sugestões de atividades físicas ( Paciente )| Médio | RF 08 | 
 RF 22 | Agendamento de consultas | Baixo | -- |



*<h3>Regras de Negócio</h3>*

Regras de Negócios| Descrição |Prioridade| Depende de.|
|:----------:|:-----------:|:------------:|:----------:|
 RN 01|O sistema deve conter autenticação de CEP e CPF|Alta|RF 01|
 RN 02|O sistema deve contar com um sistema ant-robô ( Captcha )|Alta|--|
 RN 03|O Sistema deve suportar um grande tráfego de pelo menos 1000 acessos simultâneos|Alta|--|
 RN 04|As informações guardadas em bancos de dados devem ser encriptadas|Alta|--|
 RN 05|As informações alteradas pelos usuários devem ser atualizadas no aplicativo em até 30 segundos|Média|--|
 RN 06|O sistema deve suportar informações sendo alteradas pelo Nutricionista e pelo paciente simultâneamente|Alta|--|
 RN 07|O sistema deve contar com interface Web e Mobile ( Rodar em diferentes navegadores como Chrome, Vivaldi, Opera. E sistemas Mobile como Android e IOS)|Alta|--|
 RN 08| Os dados coletados através do preenchimento dos questionarios serão utilizadas na criação dos gráficos de acompanhamento| Baixa | RF 04|
 RN 09|Deverá existir a função de excluir todas as informações de usuário do sistema|Alta|--|
 RN 10| Gráficos devem ser atualizados semanalmente| Média | RF 05|
 RN 11|Senhas de usuários deverão contar com caracteres, numerais e símbolos, totalizando pelo menos 8 dígitos na senha|Alta|--|
 RN 12| O sistema deve ser capaz de diferenciar no ato acesso, se é o nutricionista ou o paciente que está logando. | Alta | RF 02|

*<h3>Requisitos não funcionais</h3>*
Requisitos Não F. | Descrição |  Categoria |  Escopo  |Prioridade| Depende de. |
:-----------------: |:-----------:|:------------:|:----------:|:----------:|:------------:|
 RNF 01|As Informações cadastradas deverão ser guardadas em um banco dados protegido por criptografia|Segurança de acesso|Sistema|Alta|RN 01|
 RNF 02|Informações cadastradas devem ser guardadas de forma criptografada nos bancos de dados do app|Segurança de acesso|Sistema|Alta|RF 02|
 RNF 03|O sistema deve oferecer a opção de leitura, alteração e exclusão de informações cadastradas|Segurança de dados|Funcionalidade|Alta|RF 03|
 RNF 04|Sistema deve apresentar um questionário inicial contendo algumas informações no primeiro acesso|Usabilidade|Sistema|Média|RF 04|
RNF 05|O Sistema deve conter funcionalidades diferentes nas interfaces do profissional e do  paciente.|Interoperabilidade|Sistema|Alta|--|
 RNF 06|O sistema deverá contar com gráficos e dashboard para os usuários acompanharem sua evolução|Usabilidade|Sistema|Média|RF 09|
 RNF 07|O sistema deverá ter um menu com recomendações de exercícios físicos que possam corroborar com as dietas estipuladas|Usabilidade|Funcionalidade|Baixa|--|
 RNF 08|O sistema vai contar com a opção de marcar consultas online ou presenciais fora de agenda.|Atratividade|Funcionalidade|Média|--|
 RNF 10 |O sistema deve permitir aos usuários estarem efetuando LogOff do sistema perdendo assim todos os acessos às informações confidenciais.|Segurança de informação|Sistema|Alta|RF 12 |


*<h3>Prototipação de telas</h3>*

*<h4>Cadastro de usuário</h4>*

Campos|Tipo|Tamanho|
:--:|:-------:|:--:|
CPF | Texto | 11 |
Nome | Texto | Inteiro |
Endereço | Texto | Inteiro |
Telefone | Numérico | 9 |
Email |Texto | 256 |
Sexo | Texto | Inteiro |

*<h4>Login</h4>*

Campos|Tipo|Tamanho|
|:---:|:---:|:-----:|
Usuário|Texto|Inteiro|
Senha| Texto | Inteiro|

*<h4>Atualização de dados</h4>*

Campos|Tipo|Tamanho|
|:---:|:---:|:-----:|
CPF | Texto | 11 |
Nome | Texto | Inteiro |
Endereço | Texto | Inteiro |
Telefone | Numérico | 9 |
Email |Texto | 256 |
Sexo | Texto | Inteiro |

*<h4>Questionário de primeiro acesso (Paciente)</h4>*

Campos|Tipo|Tamanho|
|:---:|:---:|:-----:|
Paciente terá um questionário onde ele precisará  inserir as seguintes informações:Nome Completo, Idade, Altura, Peso, Alimentos favoritos | Texto | Inteiro |
Exames| Anexo | Inteiro |
Objetos | Texto | Inteiro |
Hábitos Alimentares | Texto | Inteiro|

*<h4>Menu com todas as funcionalidades do App</h4>*
Campos|Tipo|Tamanho|
|:---:|:---:|:-----:|
A tela deve conter um menu em formato de lista ou cascata listando todas as funcionalidades do aplicativo com botões interativos| Lista | Inteiro| 

*<h4>Criação e visualização de dieta</h4>*

Campos|Tipo|Tamanho|
|:---:|:---:|:-----:|
Na interface do Nutricionista, deve ser possível a inserção de uma dieta em formato de lista interativa. Na interface do paciente, ele deve ser capaz de visualizar as informações inseridas pelo profissional. | Texto | Inteiro

*<h4>Estipulação de Horários</h4>*
